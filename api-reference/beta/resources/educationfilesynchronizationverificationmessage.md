---
title: tipo de recurso de educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529891"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="2c9f5-105">tipo de recurso de educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="2c9f5-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c9f5-106">Representa um erro retornado ao cliente em resposta a uma solicitação para [Iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados baseada em CSV escola.</span><span class="sxs-lookup"><span data-stu-id="2c9f5-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="2c9f5-107">O recurso irá conter erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="2c9f5-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="2c9f5-108">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="2c9f5-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="2c9f5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c9f5-109">Properties</span></span>

| <span data-ttu-id="2c9f5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c9f5-110">Property</span></span> | <span data-ttu-id="2c9f5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c9f5-111">Type</span></span> | <span data-ttu-id="2c9f5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9f5-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2c9f5-113">**type**</span><span class="sxs-lookup"><span data-stu-id="2c9f5-113">**type**</span></span> | <span data-ttu-id="2c9f5-114">string</span><span class="sxs-lookup"><span data-stu-id="2c9f5-114">string</span></span> | <span data-ttu-id="2c9f5-115">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2c9f5-115">Type of the message.</span></span> <span data-ttu-id="2c9f5-116">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="2c9f5-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="2c9f5-117">**fileName**</span><span class="sxs-lookup"><span data-stu-id="2c9f5-117">**filename**</span></span> | <span data-ttu-id="2c9f5-118">string</span><span class="sxs-lookup"><span data-stu-id="2c9f5-118">string</span></span> | <span data-ttu-id="2c9f5-119">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="2c9f5-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="2c9f5-120">**description**</span><span class="sxs-lookup"><span data-stu-id="2c9f5-120">**description**</span></span> | <span data-ttu-id="2c9f5-121">string</span><span class="sxs-lookup"><span data-stu-id="2c9f5-121">string</span></span> | <span data-ttu-id="2c9f5-122">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="2c9f5-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c9f5-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c9f5-123">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
