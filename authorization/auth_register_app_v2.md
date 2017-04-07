# <a name="register-your-microsoft-graph-application-with-the-azure-ad-v20-endpoint"></a>Registrar seu aplicativo Microsoft Graph com o ponto de extremidade do Azure AD v2.0

Para usar o ponto de extremidade do Azure AD v2.0, você precisará registrar seu aplicativo no [Portal de registro do aplicativo da Microsoft](https://apps.dev.microsoft.com) (https://apps.dev.microsoft.com). Registrar seu aplicativo estabelece a identidade dele com o provedor de autenticação e permite que ele comprove a própria identidade ao enviar solicitações de autenticação do usuário. O registro gera a ID do aplicativo e o segredo do aplicativo que você usará para configurá-lo para autenticação.

> **Observação:** este artigo aborda o registro do aplicativo com o ponto de extremidade do Azure AD v2.0. Para [registrar seu aplicativo com o Azure AD](app_authorization.md), use o [Portal do Azure](https://aka.ms/aadapplist).
> 
> Além disso, lembre-se de que se você já registrou aplicativos no Portal de Gerenciamento do Microsoft Azure, esses aplicativos não estarão listados no Portal de Registro do Aplicativo. Gerencie esses aplicativos no Portal de Gerenciamento do Azure. 

1. Entre no [Portal de Registro de Aplicativos da Microsoft](https://apps.dev.microsoft.com/) usando sua conta pessoal ou uma conta corporativa ou de estudante.

2. Escolha **Adicionar um aplicativo**.

3. Insira um nome para o aplicativo e escolha **Criar aplicativo**.

    A página de registro é exibida, listando as propriedades do seu aplicativo.

4. Copie a ID do aplicativo. Esse é o identificador exclusivo do aplicativo.

    Você usará a ID do aplicativo para configurar o aplicativo.

5. Em **Plataformas**, escolha **Adicionar plataforma** e selecione a plataforma apropriada para o seu aplicativo:
    
    Para aplicativos cliente:
    1. Selecione **Plataforma móvel**.

    2. Copie a ID de cliente (ID de aplicativo) e os valores do URI de redirecionamento para a área de transferência. Você precisará inserir esses valores no exemplo de aplicativo.

        Essa ID de aplicativo é o identificador exclusivo do aplicativo. Um URI de redirecionamento é um URI exclusivo fornecido para cada aplicativo para garantir que as mensagens enviadas para esse URI sejam enviadas somente para esse aplicativo. 

    Para aplicativos Web:
    1. Selecione **Web**.
    2. Se você estiver usando o tipo de concessão Implícito ou se estiver usando o fluxo híbrido do OpenID Connect, verifique se a caixa de seleção Permitir Fluxo Implícito está marcada. 
        
        A opção Permitir Fluxo Implícito habilita o fluxo híbrido do OpenID Connect. Durante a autenticação, isso permite que o aplicativo receba informações de entrada (o id_token) e artefatos (neste caso, um código de autorização) que o aplicativo usa para obter um token de acesso.


    3. Especifique um URI de redirecionamento.
        
        O URI de redirecionamento é o local em seu aplicativo que o ponto de extremidade do Azure AD v2.0 chama quando ele processou a solicitação de autenticação.
    4. Em **Segredos do Aplicativo**, escolha **Gerar Nova Senha**. Copie o segredo do aplicativo da caixa de diálogo **Nova senha gerada**.
        
        Você usará o segredo do aplicativo para configurar o aplicativo.
    
6. Escolha **Salvar**.

## <a name="see-also"></a>Ver também

[Autenticação de aplicativo com o Microsoft Graph](auth_overview.md)
