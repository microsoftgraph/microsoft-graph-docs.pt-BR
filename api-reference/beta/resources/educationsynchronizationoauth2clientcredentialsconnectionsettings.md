---
title: recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando OAuth2 Grant de credenciais de cliente será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.
ms.openlocfilehash: 901fabb802d4ed5fa0c99538e52b9a07199eb298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038871"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="a1b01-103">recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="a1b01-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="a1b01-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1b01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1b01-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1b01-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1b01-106">Quando [OAuth2 Grant de credenciais de cliente](https://tools.ietf.org/html/rfc6749#section-4.4) será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="a1b01-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="a1b01-107">Derivado do [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a1b01-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a1b01-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1b01-108">Properties</span></span>

| <span data-ttu-id="a1b01-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1b01-109">Property</span></span> | <span data-ttu-id="a1b01-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1b01-110">Type</span></span> | <span data-ttu-id="a1b01-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1b01-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a1b01-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="a1b01-112">**tokenUrl**</span></span> | <span data-ttu-id="a1b01-113">String</span><span class="sxs-lookup"><span data-stu-id="a1b01-113">String</span></span> | <span data-ttu-id="a1b01-114">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="a1b01-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="a1b01-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="a1b01-115">**scope**</span></span> | <span data-ttu-id="a1b01-116">String</span><span class="sxs-lookup"><span data-stu-id="a1b01-116">String</span></span> | <span data-ttu-id="a1b01-117">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="a1b01-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1b01-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1b01-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
