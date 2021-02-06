---
title: Tipo de recurso userRegistrationMethodCount
description: Número de usuários registrados para um método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 8e4c19c48771ccd0bd1dd1f1a4b049334266834a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132928"
---
# <a name="userregistrationmethodcount-resource-type"></a><span data-ttu-id="583af-103">Tipo de recurso userRegistrationMethodCount</span><span class="sxs-lookup"><span data-stu-id="583af-103">userRegistrationMethodCount resource type</span></span>

<span data-ttu-id="583af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="583af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="583af-105">Número de usuários registrados para um método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="583af-105">Number of users registered for an authentication method.</span></span>

## <a name="properties"></a><span data-ttu-id="583af-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="583af-106">Properties</span></span>
|<span data-ttu-id="583af-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="583af-107">Property</span></span>|<span data-ttu-id="583af-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="583af-108">Type</span></span>|<span data-ttu-id="583af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="583af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="583af-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="583af-110">authenticationMethod</span></span>|<span data-ttu-id="583af-111">String</span><span class="sxs-lookup"><span data-stu-id="583af-111">String</span></span>|<span data-ttu-id="583af-112">Nome do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="583af-112">Name of authentication method.</span></span>|
|<span data-ttu-id="583af-113">userCount</span><span class="sxs-lookup"><span data-stu-id="583af-113">userCount</span></span>|<span data-ttu-id="583af-114">Int64</span><span class="sxs-lookup"><span data-stu-id="583af-114">Int64</span></span>|<span data-ttu-id="583af-115">Número de usuários registrados.</span><span class="sxs-lookup"><span data-stu-id="583af-115">Number of users registered.</span></span>|

## <a name="relationships"></a><span data-ttu-id="583af-116">Relações</span><span class="sxs-lookup"><span data-stu-id="583af-116">Relationships</span></span>
<span data-ttu-id="583af-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="583af-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="583af-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="583af-118">JSON representation</span></span>
<span data-ttu-id="583af-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="583af-119">The following is a JSON representation of the resource.</span></span>
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
