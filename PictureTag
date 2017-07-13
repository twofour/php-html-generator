<?php

namespace HtmlGenerator;

class PictureTag extends Markup
{
	public $options;

	/**
	 * Add a class to classList
	 * @param string $srcset Image url
	 * @param string $media Media Query
	 *                      Example: (min-width: 600px)
	 * @return static instance
	 */
	public function addSource($srcset, $media)
	{
		$this
			->addElement('source')
			->attr('srcset', $srcset)
			->attr('media', $media);

		return $this;
	}

	public function __toString()
	{
		$img = $this->addElement('img');
		$img->attributeList = $this->options;

		return parent::__toString();
	}

}
