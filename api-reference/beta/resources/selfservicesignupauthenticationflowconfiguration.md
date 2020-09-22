---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 658e27e4fe75424f4bd39cc6c3a76255e70c4d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988804"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="9868f-103">Tipo de recurso de configuração de fluxo de autenticação de autoatendimento</span><span class="sxs-lookup"><span data-stu-id="9868f-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>


<span data-ttu-id="9868f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9868f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9868f-105">Representa as configurações relacionadas ao autoatendimento de registro.</span><span class="sxs-lookup"><span data-stu-id="9868f-105">Represents the configurations related to self-service sign up.</span></span>

## <a name="properties"></a><span data-ttu-id="9868f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9868f-106">Properties</span></span>
|<span data-ttu-id="9868f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9868f-107">Property</span></span>|<span data-ttu-id="9868f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9868f-108">Type</span></span>|<span data-ttu-id="9868f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9868f-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="9868f-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9868f-110">isEnabled</span></span>|<span data-ttu-id="9868f-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="9868f-111">Boolean</span></span>|<span data-ttu-id="9868f-112">Indica se o fluxo de autoatendimento de inscrição está ativado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="9868f-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="9868f-113">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="9868f-113">The default value is `false`.</span></span> <span data-ttu-id="9868f-114">Esta propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="9868f-114">This property is not a key.</span></span> <span data-ttu-id="9868f-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9868f-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9868f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9868f-116">Relationships</span></span>
<span data-ttu-id="9868f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9868f-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9868f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9868f-118">JSON representation</span></span>
<span data-ttu-id="9868f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9868f-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
}
-->

``` json
{
  "isEnabled": "Boolean"
}
```


