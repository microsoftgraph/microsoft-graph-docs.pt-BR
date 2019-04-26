---
title: tipo de recurso educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bbf38f15fbe14112ef254c625a8747e57eb1cae4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340504"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="14e93-105">tipo de recurso educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="14e93-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14e93-106">Representa um erro retornado ao cliente em resposta a uma solicitação para [iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados escolares baseados em CSV.</span><span class="sxs-lookup"><span data-stu-id="14e93-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="14e93-107">O recurso conterá erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="14e93-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="14e93-108">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="14e93-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="14e93-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14e93-109">Properties</span></span>

| <span data-ttu-id="14e93-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14e93-110">Property</span></span> | <span data-ttu-id="14e93-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="14e93-111">Type</span></span> | <span data-ttu-id="14e93-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="14e93-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="14e93-113">**type**</span><span class="sxs-lookup"><span data-stu-id="14e93-113">**type**</span></span> | <span data-ttu-id="14e93-114">string</span><span class="sxs-lookup"><span data-stu-id="14e93-114">string</span></span> | <span data-ttu-id="14e93-115">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="14e93-115">Type of the message.</span></span> <span data-ttu-id="14e93-116">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="14e93-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="14e93-117">**nomes**</span><span class="sxs-lookup"><span data-stu-id="14e93-117">**filename**</span></span> | <span data-ttu-id="14e93-118">string</span><span class="sxs-lookup"><span data-stu-id="14e93-118">string</span></span> | <span data-ttu-id="14e93-119">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="14e93-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="14e93-120">**description**</span><span class="sxs-lookup"><span data-stu-id="14e93-120">**description**</span></span> | <span data-ttu-id="14e93-121">string</span><span class="sxs-lookup"><span data-stu-id="14e93-121">string</span></span> | <span data-ttu-id="14e93-122">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="14e93-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14e93-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14e93-123">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
