---
title: Tipo de recurso userRegistrationFeatureCount
description: Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 0a0ad3758a74e057fa5539d3d913dd1735c88854
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052553"
---
# <a name="userregistrationfeaturecount-resource-type"></a><span data-ttu-id="5119b-103">Tipo de recurso userRegistrationFeatureCount</span><span class="sxs-lookup"><span data-stu-id="5119b-103">userRegistrationFeatureCount resource type</span></span>

<span data-ttu-id="5119b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5119b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5119b-105">Representa o número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.</span><span class="sxs-lookup"><span data-stu-id="5119b-105">Represents the number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>

## <a name="properties"></a><span data-ttu-id="5119b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5119b-106">Properties</span></span>
|<span data-ttu-id="5119b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5119b-107">Property</span></span>|<span data-ttu-id="5119b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5119b-108">Type</span></span>|<span data-ttu-id="5119b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5119b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5119b-110">recurso</span><span class="sxs-lookup"><span data-stu-id="5119b-110">feature</span></span>|<span data-ttu-id="5119b-111">authenticationMethodFeature</span><span class="sxs-lookup"><span data-stu-id="5119b-111">authenticationMethodFeature</span></span>|<span data-ttu-id="5119b-112">Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.</span><span class="sxs-lookup"><span data-stu-id="5119b-112">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span> <span data-ttu-id="5119b-113">Os valores possíveis são: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span><span class="sxs-lookup"><span data-stu-id="5119b-113">Possible values are: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span></span>|
|<span data-ttu-id="5119b-114">userCount</span><span class="sxs-lookup"><span data-stu-id="5119b-114">userCount</span></span>|<span data-ttu-id="5119b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5119b-115">Int64</span></span>|<span data-ttu-id="5119b-116">Número de usuários.</span><span class="sxs-lookup"><span data-stu-id="5119b-116">Number of users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5119b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="5119b-117">Relationships</span></span>
<span data-ttu-id="5119b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5119b-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5119b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5119b-119">JSON representation</span></span>
<span data-ttu-id="5119b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5119b-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
