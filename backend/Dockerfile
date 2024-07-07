# Usa una imagen base de Odoo
FROM odoo:16.0

# Copia los módulos personalizados a la carpeta de addons de Odoo
COPY addons/* /mnt/extra-addons/

# Copia el archivo de configuración personalizado
COPY odoo.conf /etc/odoo/

# Define el usuario como odoo
USER odoo

# Comando para iniciar Odoo
CMD ["odoo", "--config=/etc/odoo/odoo.conf"]