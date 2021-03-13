---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 93b99ffc6698da60a995bdd8da8f97855dd04b1c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761062"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="0a49c-103">Tipo de recurso de configuração de fluxo de autenticação de autoatendimento</span><span class="sxs-lookup"><span data-stu-id="0a49c-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>


<span data-ttu-id="0a49c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0a49c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a49c-105">Representa as configurações relacionadas ao autoatendimento de registro.</span><span class="sxs-lookup"><span data-stu-id="0a49c-105">Represents the configurations related to self-service sign up.</span></span>

## <a name="properties"></a><span data-ttu-id="0a49c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a49c-106">Properties</span></span>
|<span data-ttu-id="0a49c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a49c-107">Property</span></span>|<span data-ttu-id="0a49c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a49c-108">Type</span></span>|<span data-ttu-id="0a49c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a49c-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="0a49c-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0a49c-110">isEnabled</span></span>|<span data-ttu-id="0a49c-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a49c-111">Boolean</span></span>|<span data-ttu-id="0a49c-112">Indica se o fluxo de autoatendimento de inscrição está ativado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="0a49c-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="0a49c-113">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="0a49c-113">The default value is `false`.</span></span> <span data-ttu-id="0a49c-114">Esta propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="0a49c-114">This property is not a key.</span></span> <span data-ttu-id="0a49c-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a49c-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0a49c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0a49c-116">Relationships</span></span>
<span data-ttu-id="0a49c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a49c-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a49c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a49c-118">JSON representation</span></span>
<span data-ttu-id="0a49c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a49c-119">The following is a JSON representation of the resource.</span></span>
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


