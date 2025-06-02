## Project v3 repositories
- [App Builder User Documentation] (https://github.com/dhjeje/BuilderHelp)
- [App Builder Web interface (frontend part, Angular 17)] (https://github.com/dhjeje/AdminPanel)
- [App Builder Core (backend part, Laravel 7, PHP8)] (https://github.com/dhjeje/Core)


### Version 2 (old)
- [App Builder Web interface (frontend part, Angular 11, previous version)] (https://github.com/dhjeje/AdminPanelOld)
- [App Builder Core, previous version (backend part, Laravel 7, PHP8)] (https://github.com/dhjeje/CoreOld)

  
## Project Setup

The project uses:
- **Frontend**: Angular 17 (new panel)
- **Backend**: Laravel 7

### Installation Instructions:

1. **Build Angular application**:
   ```bash
   ng build --prod
   ```
   Built files will be generated in the `dist/` folder

2. **Copy files to Laravel**:
   Copy builded contents from `dist/` to Laravel's `public/html/` folder

3. **Database setup**:
   - Run migrations:
     ```bash
     php artisan migrate
     ```
   - Seed initial data:
     ```bash
     php artisan db:seed
     ```

4. **Start development server**:
   ```bash
   php artisan serve
   ```

5. **Don't forget install php composer dependecies**

6. **Rename .env.example to .env**
   And add MySQL credentials

### Passwords:
admin@admin.com
manager@manager.com
user@user.com

### Notes:
- Make sure all dependencies are installed (`composer install` for Laravel, `npm install` for Angular)
- Configure your `.env` file before running migrations

### License Requirements:
Any software product derived from this source code must be licensed under the **GNU Affero General Public License (AGPL)**. This ensures that:
- All modifications must be open-sourced
- Network services using this code must provide source to users
- The same license terms must be preserved in all derivative works

See [GNU AGPL v3.0](https://www.gnu.org/licenses/agpl-3.0.html) for full license terms.
