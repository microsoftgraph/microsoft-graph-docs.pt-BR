---
title: recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando OAuth2 Grant de credenciais de cliente será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523551"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="ae36d-103">recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="ae36d-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae36d-104">Quando [OAuth2 Grant de credenciais de cliente](https://tools.ietf.org/html/rfc6749#section-4.4) será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="ae36d-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="ae36d-105">Derivado do [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ae36d-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ae36d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae36d-106">Properties</span></span>

| <span data-ttu-id="ae36d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae36d-107">Property</span></span> | <span data-ttu-id="ae36d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae36d-108">Type</span></span> | <span data-ttu-id="ae36d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae36d-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ae36d-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="ae36d-110">**tokenUrl**</span></span> | <span data-ttu-id="ae36d-111">String</span><span class="sxs-lookup"><span data-stu-id="ae36d-111">String</span></span> | <span data-ttu-id="ae36d-112">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="ae36d-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="ae36d-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="ae36d-113">**scope**</span></span> | <span data-ttu-id="ae36d-114">String</span><span class="sxs-lookup"><span data-stu-id="ae36d-114">String</span></span> | <span data-ttu-id="ae36d-115">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="ae36d-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae36d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae36d-116">JSON representation</span></span>
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
