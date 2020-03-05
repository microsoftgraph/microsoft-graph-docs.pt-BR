---
title: tipo de recurso educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 45f439adaf45ade7e63dd4cde8ed72852244192c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502001"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="94b4f-105">tipo de recurso educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="94b4f-105">educationFileSynchronizationVerificationMessage resource type</span></span>

<span data-ttu-id="94b4f-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94b4f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94b4f-107">Representa um erro retornado ao cliente em resposta a uma solicitação para [iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados escolares baseados em CSV.</span><span class="sxs-lookup"><span data-stu-id="94b4f-107">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="94b4f-108">O recurso conterá erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="94b4f-108">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="94b4f-109">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="94b4f-109">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="94b4f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94b4f-110">Properties</span></span>

| <span data-ttu-id="94b4f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94b4f-111">Property</span></span> | <span data-ttu-id="94b4f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="94b4f-112">Type</span></span> | <span data-ttu-id="94b4f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="94b4f-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="94b4f-114">**type**</span><span class="sxs-lookup"><span data-stu-id="94b4f-114">**type**</span></span> | <span data-ttu-id="94b4f-115">string</span><span class="sxs-lookup"><span data-stu-id="94b4f-115">string</span></span> | <span data-ttu-id="94b4f-116">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="94b4f-116">Type of the message.</span></span> <span data-ttu-id="94b4f-117">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="94b4f-117">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="94b4f-118">**nomes**</span><span class="sxs-lookup"><span data-stu-id="94b4f-118">**filename**</span></span> | <span data-ttu-id="94b4f-119">string</span><span class="sxs-lookup"><span data-stu-id="94b4f-119">string</span></span> | <span data-ttu-id="94b4f-120">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="94b4f-120">Source file that contains the error.</span></span> |
| <span data-ttu-id="94b4f-121">**description**</span><span class="sxs-lookup"><span data-stu-id="94b4f-121">**description**</span></span> | <span data-ttu-id="94b4f-122">string</span><span class="sxs-lookup"><span data-stu-id="94b4f-122">string</span></span> | <span data-ttu-id="94b4f-123">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="94b4f-123">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94b4f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94b4f-124">JSON representation</span></span>

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
