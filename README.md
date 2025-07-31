# yahia-maadhmoonuse App\Models\User;
use Illuminate\Support\Facades\Hash;

public function run()
{
    // Admin
    User::create([
        'name' => 'Admin User',
        'email' => 'admin@example.com',
        'password' => Hash::make('password'),
        'role' => 'admin',
    ]);

    // Agent
    User::create([
        'name' => 'Agent User',
        'email' => 'agent@example.com',
        'password' => Hash::make('password'),
        'role' => 'agent',
    ]);
}
