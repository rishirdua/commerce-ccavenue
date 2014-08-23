Commerce CCAvenue Payment Gateway Integration
=============================================
Edited the module commerce_ccavenue to make it work with the new CCAvenue multi-currency processing payment gateway. Suggestions and patches are most welcome.


Authors
--------
Rishi Dua <http://github.com/rishirdua>
Vibhav Sinha <https://github.com/vibhavsinha>


Steps to use
------------
- Install the Commerce CCAvenue (Tested on 7.x-1.2) https://www.drupal.org/project/commerce_ccavenue
- Drop into your preferred modules directory
- Enable the module from admin/build/modules
- Goto admin/commerce/config/payment-methods and create a rule for CCAvenue
- Edit Action and Configure the Working Key & Merchant ID. CCAvenue has replaced the working key with Access Code and Encryption Key. So enter Encryption Key in place of working key
- Download ccavenue.module from github.com/rishirdua/commerce-ccavenue/ and replace #value in $form['access_code'] with your Access Code.
- (Optional) Some fields are hard coded in the function ccavenue_redirect_form and should be changed if required. eg: language: EN, currency: INR, Phone number: 1234567890 etc.
- Replace the ccavenue.module file with the one in sites/all/modules/commerce_ccavenue

Contribute
----------
- Issue Tracker: https://github.com/rishirdua/commerce-ccavenue/
- Source Code: github.com/rishirdua/commerce-ccavenue
- Project page: http://rishirdua.github.io/commerce-ccavenue


LICENCE:
--------
Commerce CCAvenue Payment Gateway Integration
Copyright (C) 2014, Rishi Dua <rishirdua@gmail.com>, Vibhav Sinha <vsinha@webdweb.in>

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.