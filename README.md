# Accord\MandrillSwiftMailer

[![Build Status](https://travis-ci.org/AccordGroup/MandrillSwiftMailer.svg?branch=master)](https://travis-ci.org/AccordGroup/MandrillSwiftMailer)

A SwiftMailer transport implementation for Mandrill

## Installation

Require the package with composer

    composer require accord/mandrill-swiftmailer

## Usage
    $dispatcher = new Swift_Events_SimpleEventDispatcher();
    $transport = new MandrillTransport($dispatcher);
    $transport->setApiKey('ABCDEFG12345');
    $transport->setAsync(true); # Optional
    $transport->send($message);
