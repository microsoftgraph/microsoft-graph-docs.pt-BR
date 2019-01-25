---
title: Visão geral da API de sincronização do Azure AD
description: ') permite que você automatize a criação, manutenção e remoção de identidades em nuvem aplicativos (software como um serviço ou SaaS) como a pasta de recados, a equipe de vendas, ServiceNow e muito mais. Você pode usar a APIs de sincronização no Microsoft Graph gerenciar a sincronização de identidade programaticamente, incluindo:'
localization_priority: Normal
ms.openlocfilehash: ed994b8204fdee38f558da499259538e85eacd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529555"
---
# <a name="azure-ad-synchronization-api-overview"></a>Visão geral da API de sincronização do Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sincronização de identidades do Azure Active Directory (AD Azure) (também chamada de "provisionamento") permite automatizar a criação, manutenção e remoção de identidades em nuvem (software como um serviço ou SaaS) aplicativos, como a pasta de recados, a equipe de vendas, ServiceNow, e muito mais. Você pode usar a APIs de sincronização no Microsoft Graph gerenciar a sincronização de identidade programaticamente, incluindo:

- Criar, iniciar e interromper os trabalhos de sincronização
- Fazer alterações no esquema de sincronização para trabalhos
- Verificar o status atual da sincronização 

Para obter mais informações sobre a sincronização do Azure AD, consulte:

* [Automatizar o usuário provisionamento e desprovisionamento SaaS aplicativos com o Windows Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [Gerenciando a conta de usuário de provisionamento para aplicativos de empresa no portal do Azure](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Você também pode tentar a API do [Explorer do gráfico](https://developer.microsoft.com/graph/graph-explorer) em um locatário de amostra ou seu próprio locatário.

## <a name="synchronization-job"></a>Trabalho de sincronização

Trabalhos de sincronização realizar a sincronização periodicamente em execução em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente. O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário. Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.

Para obter mais informações, consulte o [trabalho de sincronização](synchronization-synchronizationjob.md).

## <a name="synchronization-schema"></a>Esquema de sincronização

O esquema de sincronização define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica. Normalmente, você irá personalizar alguns dos [mapeamentos de atributo](synchronization-attributemapping.md)ou adicionar um [filtro de escopo](synchronization-filter.md) para sincronizar apenas os objetos que atender a uma determinada condição.

O esquema de sincronização inclui os seguintes componentes:

- Definições do diretório
- Regras de sincronização
- Mapeamentos de objeto

Para obter mais informações, consulte [esquema de sincronização](synchronization-synchronizationschema.md).

## <a name="synchronization-template"></a>Modelo de sincronização

O modelo de sincronização fornece configurações de sincronização pré-configurado para um aplicativo específico. Essas configurações (o mais importante, o [esquema de sincronização](synchronization-synchronizationschema.md)) serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) que baseia-se no modelo. Modelos são especificados pelo desenvolvedor de aplicativos.

Para obter mais informações, consulte [modelo de sincronização](synchronization-synchronizationtemplate.md).

## <a name="working-with-the-synchronization-api"></a>Trabalhando com a API de sincronização

Trabalhando com a sincronização de API envolve principalmente a acessar os recursos [synchronizationJob](synchronization-synchronizationjob.md) e [synchronizationSchema](synchronization-synchronizationschema.md) . Para localizar seu recurso [synchronizationJob](synchronization-synchronizationjob.md) , você precisa saber a ID do objeto principal do serviço que pertence o trabalho de sincronização. Os exemplos a seguir mostram como trabalhar com os recursos **synchronizationJob** e **synchronizationSchema** .

### <a name="authorization"></a>Autorização

A API de sincronização do Azure AD usa OAuth 2.0 para autorização. Antes de fazer quaisquer solicitações da API, você precisa obter um token de acesso. Para obter mais informações, consulte [tokens de acesso de Get para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Para acessar os recursos de sincronização, seu aplicativo deve Directory.ReadWrite.All permissões. Para obter mais informações, consulte [permissões de diretório](/graph/permissions-reference#directory-permissions).

### <a name="find-the-service-principal-object-by-display-name"></a>Localizar o objeto de entidade de serviço por nome para exibição

O exemplo a seguir mostra como localizar o objeto de entidade de serviço por nome para exibição.

Solicitação 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

**Response**

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a>Localizar o objeto de entidade de serviço por ID de aplicativo

O exemplo a seguir mostra como localizar o objeto de entidade de serviço por ID de aplicativo.

Solicitação
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

Resposta
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a>Listar os trabalhos de sincronização existente

O exemplo a seguir mostra como listar os trabalhos de sincronização existente.

Solicitação
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

Resposta
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a>Obter o status do trabalho de sincronização
O exemplo a seguir mostra como obter o status de um trabalho de sincronização.

Solicitação
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

Resposta
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a>Obter o esquema de sincronização
O exemplo a seguir mostra como obter o esquema de sincronização.

Solicitação
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

Resposta
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>Confira também

* [Configurar a sincronização com os atributos de extensão de diretório](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [Configurar a sincronização com atributos personalizados de destino](../resources/synchronization-configure-with-custom-target-attributes.md)



<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
