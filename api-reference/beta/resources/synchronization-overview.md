---
title: Visão geral da API de sincronização do Azure AD
description: Automatize o provisionamento de identidades de sistemas de RH, Active Directory e Azure Active Directory para aplicativos em nuvem.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a08be511c3752e27f2e86415aee62d112d2c5262
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133158"
---
# <a name="azure-ad-synchronization-api-overview"></a>Visão geral da API de sincronização do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A sincronização de identidade do Azure Active Directory (Azure AD) (também chamada de "provisionamento") permite automatizar o provisionamento (criação, manutenção) e o des provisionamento (remoção) de identidades de qualquer um dos seguintes:
- Active Directory para Azure AD
- Dia de trabalho para o Azure AD
- Azure AD para aplicativos de nuvem como Dropbox, Salesforce, ServiceNow e muito mais 

Você pode usar as APIs de sincronização  no Microsoft Graph para gerenciar a sincronização de identidade programaticamente, incluindo:

- Criar, iniciar e interromper trabalhos de sincronização
- Fazer alterações no esquema de sincronização para trabalhos
- Status de sincronização atual.

Para saber mais sobre a sincronização no Azure AD, confira:

* [Automatizar o provisionamento e o desprovisionamento de usuários para aplicativos SaaS com o Azure Active Directory](/azure/active-directory/active-directory-saas-app-provisioning)
* [Gerenciando o provisionamento de conta de usuário para aplicativos corporativos no portal do Azure](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Você também pode experimentar a API no Explorador do [Graph em](https://developer.microsoft.com/graph/graph-explorer) um locatário de exemplo ou em seu próprio locatário.

## <a name="synchronization-job"></a>Trabalho de sincronização

Os trabalhos de sincronização executam a sincronização periodicamente em segundo plano, sondando alterações em um diretório e os pressionando para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.

Para obter mais informações, consulte [o trabalho de sincronização.](synchronization-synchronizationjob.md)

## <a name="synchronization-schema"></a>Esquema de sincronização

O esquema de sincronização define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de configuração para um trabalho de sincronização específico. Normalmente, você personalizará alguns dos [mapeamentos](synchronization-attributemapping.md)de atributos ou adicionará um filtro de [scoping](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.

O esquema de sincronização inclui os seguintes componentes:

- Definições de diretório
- Regras de sincronização
- Mapeamentos de objetos

Para obter mais informações, [consulte o esquema de sincronização.](synchronization-synchronizationschema.md)

## <a name="synchronization-template"></a>Modelo de sincronização

O modelo de sincronização fornece configurações de sincronização pré-configuradas para um aplicativo específico. Essas configurações (o mais [importante,](synchronization-synchronizationschema.md)esquema de sincronização [](synchronization-synchronizationjob.md) ) serão usadas por padrão para qualquer trabalho de sincronização baseado no modelo. Os modelos são especificados pelo desenvolvedor do aplicativo.

Para obter mais informações, consulte [o modelo de sincronização.](synchronization-synchronizationtemplate.md)

## <a name="working-with-the-synchronization-api"></a>Trabalhando com a API de sincronização

Trabalhar com a API de sincronização envolve principalmente o acesso aos recursos [synchronizationJob](synchronization-synchronizationjob.md) e [synchronizationSchema.](synchronization-synchronizationschema.md) Para encontrar o [recurso synchronizationJob,](synchronization-synchronizationjob.md) você precisa saber a ID do objeto de entidade de serviço ao qual o trabalho de sincronização pertence. Os exemplos a seguir mostram como trabalhar com os recursos **synchronizationJob** e **synchronizationSchema.**

### <a name="authorization"></a>Autorização

A API de sincronização do Azure AD usa o OAuth 2.0 para autorização. Antes de fazer solicitações à API, você precisa obter um token de acesso. Para saber mais, confira [Obter tokens de acesso para chamar o Microsoft Graph.](/graph/auth/) Para acessar os recursos de sincronização, seu aplicativo precisa de permissões Directory.ReadWrite.All. Para obter mais informações, consulte [Permissões de diretório.](/graph/permissions-reference#directory-permissions)

### <a name="find-the-service-principal-object-by-display-name"></a>Encontrar o objeto de entidade de serviço por nome de exibição

O exemplo a seguir mostra como encontrar o objeto de entidade de serviço pelo nome de exibição.

**Solicitação**

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

### <a name="find-the-service-principal-object-by-app-id"></a>Encontre o objeto da entidade de serviço por ID do aplicativo

O exemplo a seguir mostra como encontrar o objeto de entidade de serviço por ID do aplicativo.

**Solicitação**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

**Response**
<!-- { "blockType": "ignored" } -->
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

### <a name="list-existing-synchronization-jobs"></a>Listar trabalhos de sincronização existentes

O exemplo a seguir mostra como listar trabalhos de sincronização existentes.

**Solicitação**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

**Response**
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-job-status"></a>Obter status do trabalho de sincronização
O exemplo a seguir mostra como obter o status de um trabalho de sincronização.

**Solicitação**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

**Response**
<!-- { "blockType": "ignored" } -->
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

### <a name="get-synchronization-schema"></a>Obter esquema de sincronização
O exemplo a seguir mostra como obter o esquema de sincronização.

**Solicitação**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

**Response**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>Confira também

* [Configurar a sincronização com atributos de extensão de diretório](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [Configurar a sincronização com atributos de destino personalizados](../resources/synchronization-configure-with-custom-target-attributes.md)
