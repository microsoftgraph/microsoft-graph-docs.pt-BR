---
title: tipo de recurso userFlowApiConnectorConfiguration
description: Representa quais conectores de API estão habilitados para um fluxo de usuário.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 00b37f1b4bff0edf8aa85d79a01e23169b45dbcf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720097"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="08553-103">tipo de recurso userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="08553-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="08553-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08553-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08553-105">Define quais APIs são chamadas em pontos específicos no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="08553-105">Defines which APIs are called at specific points in the user flow.</span></span>  <span data-ttu-id="08553-106">Cada relação desse objeto corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.</span><span class="sxs-lookup"><span data-stu-id="08553-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="08553-107">Relações</span><span class="sxs-lookup"><span data-stu-id="08553-107">Relationships</span></span>

| <span data-ttu-id="08553-108">Relação</span><span class="sxs-lookup"><span data-stu-id="08553-108">Relationship</span></span>            | <span data-ttu-id="08553-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="08553-109">Type</span></span>                                            | <span data-ttu-id="08553-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="08553-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="08553-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="08553-111">postFederationSignup</span></span>    | [<span data-ttu-id="08553-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="08553-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="08553-113">Especifica uma API a ser chamada após a Federação com um provedor de identidade externo (como Google, Facebook ou Azure AD) é concluída quando o usuário está se inscrevendo (não se aplica à entrada).</span><span class="sxs-lookup"><span data-stu-id="08553-113">Specifies an API to call after federation with an external identity provider (like Google, Facebook, or Azure AD) is completed when user is signing up (does not apply to sign in).</span></span> |
| <span data-ttu-id="08553-114">setattributecollection</span><span class="sxs-lookup"><span data-stu-id="08553-114">postAttributeCollection</span></span> | [<span data-ttu-id="08553-115">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="08553-115">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="08553-116">Especifica uma API para chamar após um usuário enviar os atributos coletados e antes de o usuário ser criado durante a inscrição.</span><span class="sxs-lookup"><span data-stu-id="08553-116">Specifies an API to call after a user submits collected attributes and before the user is created during sign up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="08553-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08553-117">JSON representation</span></span>

<span data-ttu-id="08553-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08553-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowApiConnectorConfiguration"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "User flow API Connector Configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: Resource userFlowApiConnectorConfiguration has documented navigation properties, but we thought it was a complex type!"
  ]
}-->
