---
title: recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando OAuth2 Grant de credenciais de cliente será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
ms.openlocfilehash: 49a0a267ddb3a8f3a954888679806ea7913e24f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822579"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="87812-103">recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="87812-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="87812-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87812-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87812-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87812-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87812-106">Quando [OAuth2 Grant de credenciais de cliente](https://tools.ietf.org/html/rfc6749#section-4.4) será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.</span><span class="sxs-lookup"><span data-stu-id="87812-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="87812-107">Derivado do [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="87812-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87812-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87812-108">Properties</span></span>

| <span data-ttu-id="87812-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87812-109">Property</span></span> | <span data-ttu-id="87812-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="87812-110">Type</span></span> | <span data-ttu-id="87812-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87812-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="87812-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="87812-112">**tokenUrl**</span></span> | <span data-ttu-id="87812-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87812-113">String</span></span> | <span data-ttu-id="87812-114">A URL para obter tokens de acesso para o provedor de dados.</span><span class="sxs-lookup"><span data-stu-id="87812-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="87812-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="87812-115">**scope**</span></span> | <span data-ttu-id="87812-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87812-116">String</span></span> | <span data-ttu-id="87812-117">[O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="87812-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87812-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87812-118">JSON representation</span></span>
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
