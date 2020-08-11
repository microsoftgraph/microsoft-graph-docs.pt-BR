---
title: Visão geral da API de sincronização do Azure AD
description: Automatizar o provisionamento de identidades de sistemas de RH, Active Directory e Azure Active Directory para aplicativos em nuvem.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d1a2de9dcac9765899fa3eaff6173a3791984ade
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630316"
---
# <a name="azure-ad-synchronization-api-overview"></a>Visão geral da API de sincronização do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A sincronização de identidade do Azure Active Directory (Azure AD) (também chamada de "provisionamento") permite automatizar o provisionamento (criação, manutenção) e desprovisionamento (remoção) de identidades de qualquer um dos seguintes:
- Active Directory para o Azure AD
- WORKDAY para o Azure AD
- Azure AD para aplicativos em nuvem como o Dropbox, Salesforce, ServiceNow e muito mais 

Você pode usar as APIs de sincronização no Microsoft Graph para gerenciar a sincronização de identidade de forma programática, incluindo:

- Criar, iniciar e interromper trabalhos de sincronização
- Fazer alterações no esquema de sincronização para trabalhos
- Verificar o status de sincronização atual

Para obter mais informações sobre sincronização no Azure AD, consulte:

* [Automatizar o provisionamento de usuários e desprovisionamento para aplicativos SaaS com o Azure Active Directory](/azure/active-directory/active-directory-saas-app-provisioning)
* [Gerenciando o provisionamento de contas de usuário para aplicativos corporativos no portal do Azure](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Você também pode experimentar a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) em um locatário de exemplo ou seu próprio locatário.

## <a name="synchronization-job"></a>Trabalho de sincronização

Os trabalhos de sincronização realizam a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório. O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário. Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.

Para obter mais informações, consulte [trabalho de sincronização](synchronization-synchronizationjob.md).

## <a name="synchronization-schema"></a>Esquema de sincronização

O esquema de sincronização define quais objetos serão sincronizados e como eles serão sincronizados. O esquema de sincronização contém a maioria das informações de configuração de um determinado trabalho de sincronização. Normalmente, você personalizará alguns dos [mapeamentos de atributo](synchronization-attributemapping.md)ou adicionará um [filtro de escopo](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.

O esquema de sincronização inclui os seguintes componentes:

- Definições de diretório
- Regras de sincronização
- Mapeamentos de objetos

Para obter mais informações, consulte [Synchronization Schema](synchronization-synchronizationschema.md).

## <a name="synchronization-template"></a>Modelo de sincronização

O modelo de sincronização fornece configurações de sincronização pré-configuradas para um aplicativo específico. Essas configurações (mais importante, [esquema de sincronização](synchronization-synchronizationschema.md)) serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) baseado no modelo. Os modelos são especificados pelo desenvolvedor do aplicativo.

Para obter mais informações, consulte [modelo de sincronização](synchronization-synchronizationtemplate.md).

## <a name="working-with-the-synchronization-api"></a>Trabalhar com a API de sincronização

O trabalho com a API de sincronização envolve principalmente o acesso aos recursos do [synchronizationJob](synchronization-synchronizationjob.md) e do [synchronizationSchema](synchronization-synchronizationschema.md) . Para localizar o recurso [synchronizationJob](synchronization-synchronizationjob.md) , você precisa saber a ID do objeto de entidade de serviço ao qual o trabalho de sincronização pertence. Os exemplos a seguir mostram como trabalhar com os recursos **synchronizationJob** e **synchronizationSchema** .

### <a name="authorization"></a>Autorização

A API de sincronização do Azure AD usa o OAuth 2,0 para autorização. Antes de fazer qualquer solicitação para a API, você precisa obter um token de acesso. Para obter mais informações, consulte [obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Para acessar os recursos de sincronização, seu aplicativo precisa de permissões de Directory. ReadWrite. All. Para obter mais informações, consulte [Directory Permissions](/graph/permissions-reference#directory-permissions).

### <a name="find-the-service-principal-object-by-display-name"></a>Localizar o objeto de entidade de serviço por nome de exibição

O exemplo a seguir mostra como localizar o objeto de entidade de serviço por nome de exibição.

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

### <a name="find-the-service-principal-object-by-app-id"></a>Localizar o objeto de entidade de serviço por ID de aplicativo

O exemplo a seguir mostra como localizar o objeto de entidade de serviço por ID de aplicativo.

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

O exemplo a seguir mostra como listar os trabalhos de sincronização existentes.

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

### <a name="get-synchronization-job-status"></a>Obter o status do trabalho de sincronização
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



