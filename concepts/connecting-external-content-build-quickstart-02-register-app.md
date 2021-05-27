<!-- markdownlint-disable MD002 MD041 -->

Depois de todos os pré-requisitos, você poderá registrar um aplicativo no centro de administração do Azure AD. O registro é necessário para autenticar o aplicativo e usá-lo para fazer chamadas para a API de conectores Graph Microsoft.

1. Vá para o Azure Active Directory [de administração e](https://aad.portal.azure.com/) entre com uma conta de administrador.
2. No painel esquerdo, selecione **Azure Active Directory**, e em **Gerenciar**, selecione Registros **de aplicativo.**
3. Selecione **Novo registro**.

    ![Captura de tela mostrando a seção "registros de aplicativo"](images/connectors-images/build2.png)

4. Conclua **o formulário Registrar um** aplicativo com os seguintes valores e selecione **Registrar**.

    a. **Nome**: Conector de Inventário de Partes

    b. **Tipos de conta com suporte:** Contas somente neste diretório organizacional (somente microsoft - locatário único)

    c. **URI de redirecionamento**: deixar em branco

    ![Captura de tela mostrando a seção "registrar um aplicativo"](images/connectors-images/build3-contoso-register-app.png)

5. Na página Visão geral do Conector de Inventário de Partes, copie os valores de ID de Aplicativo (cliente) e ID de Diretório **(locatário).** Você precisará dos dois na seção a seguir.

    ![Captura de tela mostrando a seção "conector de inventário de partes"](images/connectors-images/build3-contoso-partsinv.png)

6. Selecione **Permissões de API em** **Gerenciar**.
7. Selecione **Adicionar uma permissão** e selecione Microsoft **Graph**.
8. Selecione **Permissões de aplicativo** e selecione a permissão **ExternalItem.ReadWrite.All.** Selecione **Adicionar permissões**.

    ![Captura de tela mostrando a seção "solicitar permissões de API"](images/connectors-images/build4.png)

9. Selecione **Conceder consentimento de administrador para {TENANT}e** selecione **Sim** quando solicitado.

    ![Captura de tela mostrando a seção "permissões de api do conector de inventário de partes"](images/connectors-images/build5.png)

10. Selecione **Certificados &amp; segredos em** **Gerenciar** , em seguida, selecione Novo segredo **do cliente**.
11. Insira uma descrição e escolha um tempo de expiração para o segredo e selecione **Adicionar**.

    ![Captura de tela mostrando a seção "certificados e segredos do conector de inventário de partes"](images/connectors-images/build6.png)

12. Copie e salve o novo segredo, você precisará dele na seção a seguir.
