---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507032"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="54166-103">recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="54166-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54166-104">Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="54166-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="54166-105">Derivado de [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="54166-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="54166-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54166-106">Properties</span></span>

| <span data-ttu-id="54166-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54166-107">Property</span></span> | <span data-ttu-id="54166-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="54166-108">Type</span></span> | <span data-ttu-id="54166-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="54166-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="54166-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="54166-110">**tokenUrl**</span></span> | <span data-ttu-id="54166-111">String</span><span class="sxs-lookup"><span data-stu-id="54166-111">String</span></span> | <span data-ttu-id="54166-112">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="54166-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="54166-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="54166-113">**scope**</span></span> | <span data-ttu-id="54166-114">String</span><span class="sxs-lookup"><span data-stu-id="54166-114">String</span></span> | <span data-ttu-id="54166-115">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="54166-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54166-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54166-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth2clientcredentialsconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
