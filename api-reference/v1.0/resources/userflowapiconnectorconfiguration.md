---
title: Tipo de recurso userFlowApiConnectorConfiguration
description: Representa os conectores de API habilitados para um fluxo de usuários.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b9d9b87bf59a796e8c79875a8506fccdd4d3447b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882798"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="741b2-103">Tipo de recurso userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="741b2-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="741b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="741b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="741b2-105">Define as APIs que são chamadas em pontos específicos no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="741b2-105">Defines the APIs that are called at specific points in the user flow.</span></span>  <span data-ttu-id="741b2-106">Cada relação desse objeto corresponde a uma etapa específica no fluxo do usuário que pode ser configurada para chamar um conector de API.</span><span class="sxs-lookup"><span data-stu-id="741b2-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="741b2-107">Relações</span><span class="sxs-lookup"><span data-stu-id="741b2-107">Relationships</span></span>

| <span data-ttu-id="741b2-108">Relação</span><span class="sxs-lookup"><span data-stu-id="741b2-108">Relationship</span></span>            | <span data-ttu-id="741b2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="741b2-109">Type</span></span>                                            | <span data-ttu-id="741b2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="741b2-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="741b2-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="741b2-111">postFederationSignup</span></span>    | [<span data-ttu-id="741b2-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="741b2-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="741b2-113">Especifica uma API a ser chamada após a federação com um provedor de identidade externo.</span><span class="sxs-lookup"><span data-stu-id="741b2-113">Specifies an API to call after federation with an external identity provider.</span></span> <span data-ttu-id="741b2-114">Por exemplo, uma API do Google, Facebook ou Azure AD é concluída quando o usuário está se insinuando (não se aplica à inscrição).</span><span class="sxs-lookup"><span data-stu-id="741b2-114">For example, a Google, Facebook, or Azure AD API is completed when the user is signing up (does not apply to sign-in).</span></span> |
| <span data-ttu-id="741b2-115">postAttributeCollection</span><span class="sxs-lookup"><span data-stu-id="741b2-115">postAttributeCollection</span></span> | [<span data-ttu-id="741b2-116">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="741b2-116">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="741b2-117">Especifica uma API a ser chamada depois que um usuário envia os atributos coletados e antes que a conta de usuário seja criada durante a assinatura.</span><span class="sxs-lookup"><span data-stu-id="741b2-117">Specifies an API to call after a user submits the collected attributes and before the user account is created during sign-up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="741b2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="741b2-118">JSON representation</span></span>

<span data-ttu-id="741b2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="741b2-119">The following is a JSON representation of the resource.</span></span>
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
  ]
}-->
