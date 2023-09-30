<?php
class TextformatterUnentities extends WireData implements Textformatter {
    public static function getModuleInfo() {
        return [
            'title' => 'Textformatter Unentities',
            'version' => 1,
            'summary' => 'Convert HTML entities back to their original characters.',
            'autoload' => true,
            'singular' => true,
        ];
    }

    public function format(Page $page, $text, $options = array()) {
        $sanitizer = $this->wire('sanitizer');
        return $sanitizer->unentities($text);
    }
}