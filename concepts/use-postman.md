---
title: Use o Postman com a API do Microsoft Graph
description: Use a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.
author: ''
localization_priority: Priority
ms.openlocfilehash: 2140dec07328b75f7b1729cd3e7cf7c86e65f738
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038182"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>Use o Postman com a API do Microsoft Graph

Você pode usar a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.

![Imagem do Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

Este artigo explica como começar a usar o Postman e o Microsoft Graph. Você também pode explorar as APIs do Microsoft Graph diretamente em seu navegador da Web usando o [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer).

## <a name="accessing-the-collection"></a>Acessando a coleção
Você pode acessar a coleção no Postman de duas maneiras: adquirindo-o ou contribuindo para ele. Primeiro, o [Postman](https://www.getpostman.com/) precisará estar em execução no seu computador.

### <a name="consume-the-collection"></a>Adquirir a coleção
Adquirir a coleção é a maneira mais fácil de começar a usar as APIs do Microsoft Graph. O [link de compartilhamento do Postman](https://www.getpostman.com/collections/d89a737b5f0c0825898a) iniciará o Postman.

A vantagem de usar a coleção compartilhada é que novas solicitações serão exibidas automaticamente, sem a necessidade de etapas adicionais.

Após obter a coleção, você precisará configurar as variáveis do ambiente:

1. Selecione **Arquivo | Importar ...**.
2. Selecione **Importar do link**.
3. Copie e cole o seguinte URL e selecione **Importar**.
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json
    ```

Você deverá ver o **ambiente do Microsoft Graph** na lista suspensa do ambiente na parte superior direita, próximo ao ícone de olho. Agora, você precisará [configurar o seu ambiente](#using-the-collection).

### <a name="contribute-to-the-collection"></a>Contribua para a coleção
Se você desejar contribuir com suas próprias solicitações, você precisará bifurcar o repositório github das [coleções do Microsoft Graph Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections). 

Para detalhes sobre como fazer isso, assista ao vídeo a seguir.

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

Para importar as coleções do Postman:

1. Baixe e registre-se no [Postman](https://www.getpostman.com/).
2. Selecione **Arquivo | Importar ...**.
3. Selecione **Importar do link**.
4. Cole os dois URLs a seguir e selecione **Importar** após cada um.

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json

    ```

Você deverá ver a coleção do **Microsoft Graph v1.0** no painel **Coleções**.

## <a name="using-the-collection"></a>Usando a coleção
Após obter a coleção do **Microsoft Graph v1.0** e o **ambiente do Microsoft Graph** no Postman, siga estas etapas.

### <a name="set-up-application-api-calls"></a>Configure as chamadas de API do aplicativo

1. Escolha a opção **Sem ambiente** na lista suspensa na parte superior direita.
2. Selecione **ambiente do Microsoft Graph**.
3. Selecione o ícone de **olho** à direita e, em seguida, **Editar**.
4. Insira o seu aplicativo da plataforma de identidade da Microsoft nas variáveis **atuais** (e não **iniciais**): **ClientID**, **ClientSecret** e **TenantID**. 
 Para obter mais informações sobre como criar um aplicativo e autorizar o fluxo único do aplicativo, confira a postagem do blog [Usar o Postman para fazer chamadas do Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/).

5. Selecione **Atualizar**. Feche a caixa de diálogo **Gerenciar Ambientes**. Na coleção do **Microsoft Graph v1.0 | Aplicativo** no lado esquerdo, selecione **Obter Token de Acesso Único do Aplicativo**. Em seguida, no lado direito, selecione **Enviar**.
6. Expanda a pasta **Aplicativo | Usuários** e selecione **Obter Usuários**. Em seguida, clique em **Enviar**.

Agora você está pronto para usar as coleções do Microsoft Graph v1.0.

>**Observação:** se você deseja executar outras APIs na coleção, você precisará concordar com as permissões necessárias do seu aplicativo.

### <a name="set-up-on-behalf-of-api-calls"></a>Configurar as chamadas de API em nome de
A maneira mais simples de configurar chamadas de APIs em nome de é fornecer um **UserName** e **UserPassword** nas configurações de ambiente e usar o **Em Nome de um Usuário | Obter Token de Acesso do Usuário**. 

>**Importante:** não recomendamos o uso de contas de usuário de produção, pois essas informações são armazenadas diretamente no Postman. Também não recomendamos o uso deste método para obter tokens de acesso na produção. Use-o apenas para fins de teste.

Se você não deseja armazenar nomes de usuário e senhas em variáveis de ambiente que sincronizam com a sua conta de nuvem do Postman, é possível usar a função **Obter Novo Token de Acesso** para obter um token sem sair do Postman.

1. Selecione **Em nome de um Usuário | Obter Token de Acesso usando o Postman**.
2. Selecione a guia **Autorização**.
3. Selecione o botão **obter token de acesso**.
4. Preencha os campos a seguir com os seus valores reais de locatário e aplicativo. Note que aqui você não poderá usar as variáveis de ambiente; você terá que usar os valores reais. Eles podem ser encontrados selecionando **EndPoints** na lâmina do aplicativo em portal.azure.com.

    - URL de retorno de chamada: https://app.getpostman.com/oauth2/callback
    - URL de Autenticação: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize
    - URL do Token de Acesso: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token
    - ID do Cliente: **CLIENTID**
    - Segredo do Cliente: **CLIENTSECRET**
    - Escopo: https://graph.microsoft.com/.default
    - Estado: **RANDOMSTRING**
 
5. Selecione **Solicitar Token**. Você deverá ver um prompt de interface de usuário para entrar e autorizar permissões.
6. Copie o token de acesso, abra as suas variáveis de ambiente e cole-o no campo **UserAccessToken**.

Agora todas as suas solicitações irão funcionar.
