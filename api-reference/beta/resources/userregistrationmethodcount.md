---
title: Tipo de recurso userRegistrationMethodCount
description: Número de usuários registrados para um método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: b61cb0448c131fc49df43154522e587644d13dc6
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052559"
---
# <a name="userregistrationmethodcount-resource-type"></a><span data-ttu-id="b79f9-103">Tipo de recurso userRegistrationMethodCount</span><span class="sxs-lookup"><span data-stu-id="b79f9-103">userRegistrationMethodCount resource type</span></span>

<span data-ttu-id="b79f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b79f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b79f9-105">Número de usuários registrados para um método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b79f9-105">Number of users registered for an authentication method.</span></span>

## <a name="properties"></a><span data-ttu-id="b79f9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b79f9-106">Properties</span></span>
|<span data-ttu-id="b79f9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b79f9-107">Property</span></span>|<span data-ttu-id="b79f9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b79f9-108">Type</span></span>|<span data-ttu-id="b79f9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b79f9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b79f9-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b79f9-110">authenticationMethod</span></span>|<span data-ttu-id="b79f9-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b79f9-111">String</span></span>|<span data-ttu-id="b79f9-112">Nome do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b79f9-112">Name of authentication method.</span></span>|
|<span data-ttu-id="b79f9-113">userCount</span><span class="sxs-lookup"><span data-stu-id="b79f9-113">userCount</span></span>|<span data-ttu-id="b79f9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b79f9-114">Int64</span></span>|<span data-ttu-id="b79f9-115">Número de usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="b79f9-115">Number of users registered.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b79f9-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b79f9-116">Relationships</span></span>
<span data-ttu-id="b79f9-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b79f9-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b79f9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b79f9-118">JSON representation</span></span>
<span data-ttu-id="b79f9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b79f9-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```