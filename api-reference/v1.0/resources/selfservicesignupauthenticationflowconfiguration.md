---
title: Tipo de recurso de configuração de fluxo de autenticação de autoatendimento
description: Representa as configurações relacionadas ao autoatendimento de inscrição.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a235c9e9869b3e0b0c36b0369ae6163083b3cf20
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882799"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="ea7ab-103">Tipo de recurso de configuração de fluxo de autenticação de autoatendimento</span><span class="sxs-lookup"><span data-stu-id="ea7ab-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>

<span data-ttu-id="ea7ab-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ea7ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea7ab-105">Representa as configurações relacionadas a inscrição de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="ea7ab-105">Represents the configurations related to self-service sign-up.</span></span>

## <a name="properties"></a><span data-ttu-id="ea7ab-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea7ab-106">Properties</span></span>

|<span data-ttu-id="ea7ab-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea7ab-107">Property</span></span>|<span data-ttu-id="ea7ab-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea7ab-108">Type</span></span>|<span data-ttu-id="ea7ab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea7ab-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="ea7ab-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ea7ab-110">isEnabled</span></span>|<span data-ttu-id="ea7ab-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea7ab-111">Boolean</span></span>|<span data-ttu-id="ea7ab-112">Indica se o fluxo de autoatendimento de inscrição está ativado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="ea7ab-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="ea7ab-113">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="ea7ab-113">The default value is `false`.</span></span> <span data-ttu-id="ea7ab-114">Esta propriedade não é uma chave.</span><span class="sxs-lookup"><span data-stu-id="ea7ab-114">This property is not a key.</span></span> <span data-ttu-id="ea7ab-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea7ab-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ea7ab-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ea7ab-116">Relationships</span></span>

<span data-ttu-id="ea7ab-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea7ab-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea7ab-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea7ab-118">JSON representation</span></span>

<span data-ttu-id="ea7ab-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea7ab-119">The following is a JSON representation of the resource.</span></span>
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
