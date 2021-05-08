---
title: Tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4c5da3180b1c15f2363bfd651d0f4e3d68f41b60
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232128"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="8219a-103">Tipo de recurso educationOnPremisesInfo</span><span class="sxs-lookup"><span data-stu-id="8219a-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="8219a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8219a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8219a-105">Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8219a-105">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="8219a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8219a-106">Properties</span></span>

| <span data-ttu-id="8219a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8219a-107">Property</span></span>    | <span data-ttu-id="8219a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8219a-108">Type</span></span>   | <span data-ttu-id="8219a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8219a-109">Description</span></span>                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| <span data-ttu-id="8219a-110">immutableId</span><span class="sxs-lookup"><span data-stu-id="8219a-110">immutableId</span></span> | <span data-ttu-id="8219a-111">String</span><span class="sxs-lookup"><span data-stu-id="8219a-111">String</span></span> | <span data-ttu-id="8219a-112">Identificador exclusivo do objeto do usuário no Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8219a-112">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8219a-113">Relações</span><span class="sxs-lookup"><span data-stu-id="8219a-113">Relationships</span></span>

<span data-ttu-id="8219a-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8219a-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8219a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8219a-115">JSON representation</span></span>

<span data-ttu-id="8219a-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8219a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOnPremisesInfo",
  "immutableId": "String"
}
```
