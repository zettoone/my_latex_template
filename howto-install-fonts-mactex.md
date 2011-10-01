# Installing TeX fonts with MacTeX

This is a brief version of the doc [Installing TeX fonts](http://tug.org/fonts/fontinstall.html).

I simply noted down how I got things down in my mac, and I won't make any guarantee to others...XD

1. first of all, get your desired font package from CTAN;
2. locate your texmf-local directory by 

   kpsewhich --var-value TEXMFLOCAL

3. uppack your package in texfm-local directory (if your package is properly organized...)

4. Run the following command to update the "TeX filename database"

   sudo -H mktexlsr

5. Map files with the information about your new font

   sudo -H updmap-sys --enable Map=*newfont.map*

6. In my case, I have to rumake the filename database again

    sudo -H mktexlsr

That's how I got things done!
