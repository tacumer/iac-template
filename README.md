 status = event['pathParameters']['status']
              return {
                  'statusCode': 200,
                  'body': {
                      'message': f'GET: Successfully accessed /v1/notify/{status}/abc',
                      'status': status
                  }
              }





 status = event['pathParameters']['status']
              body = json.loads(event.get('body', '{}'))
              return {
                  'statusCode': 200,
                  'body': json.dumps({
                      'message': f'POST: Successfully accessed /v1/notify/{status}/abc',
                      'status': status,
                      'input': body
                  })
              }
