# ansible-tower-mock

A simple script to mock launching ansible-tower job templates

## How to run

1. Copy the script into your playbooks folder
2. Set `FLASK_APP` to `ansible-tower-mock.py`
3. Set `MOCK_PLAYBOOK` to the path of your playbook
4. Run `flask run`

You can then make POST requests to `/api/v2/job_templates/<job_template_id>/launch/` and
the script will run `ansible-playbook` locally in the folder.
