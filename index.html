// database setup
const SUPABASE_URL = 'https://jkqayyoyrzmrscqjkeqr.supabase.co';
const SUPABASE_ANON_KEY = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImprcWF5eW95cnptcnNjcWprZXFyIiwicm9sZSI6ImFub24iLCJpYXQiOjE3Nzc2MTE3MjYsImV4cCI6MjA5MzE4NzcyNn0.IEsgMQsD5Sq4heWsmafHowKLh1KfXU___DcPBDATv38';
const supabaseClient = supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);

/**
 * hashes strings so we never store plain-text names or passwords.
 * this is the "zero-knowledge" part of openvault.
 */
async function generateHash(text) {
    const msgUint8 = new TextEncoder().encode(text.toLowerCase().trim());
    const hashBuffer = await crypto.subtle.digest('SHA-256', msgUint8);
    return Array.from(new Uint8Array(hashBuffer))
        .map(b => b.toString(16).padStart(2, '0'))
        .join('');
}

// export these to be used by our react ui
window.VaultEngine = {
    client: supabaseClient,
    hash: generateHash,
    storageUrl: `${SUPABASE_URL}/storage/v1/object/public/vaults/`
};
