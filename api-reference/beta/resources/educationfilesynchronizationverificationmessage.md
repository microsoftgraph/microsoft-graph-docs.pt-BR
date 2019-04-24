---
title: tipo de recurso educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados escolares baseados em CSV. O recurso conterá erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507102"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="20bfb-105">tipo de recurso educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="20bfb-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20bfb-106">Representa um erro retornado ao cliente em resposta a uma solicitação para [iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados escolares baseados em CSV.</span><span class="sxs-lookup"><span data-stu-id="20bfb-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="20bfb-107">O recurso conterá erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="20bfb-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="20bfb-108">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="20bfb-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="20bfb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20bfb-109">Properties</span></span>

| <span data-ttu-id="20bfb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20bfb-110">Property</span></span> | <span data-ttu-id="20bfb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="20bfb-111">Type</span></span> | <span data-ttu-id="20bfb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="20bfb-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="20bfb-113">**type**</span><span class="sxs-lookup"><span data-stu-id="20bfb-113">**type**</span></span> | <span data-ttu-id="20bfb-114">string</span><span class="sxs-lookup"><span data-stu-id="20bfb-114">string</span></span> | <span data-ttu-id="20bfb-115">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="20bfb-115">Type of the message.</span></span> <span data-ttu-id="20bfb-116">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="20bfb-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="20bfb-117">**nomes**</span><span class="sxs-lookup"><span data-stu-id="20bfb-117">**filename**</span></span> | <span data-ttu-id="20bfb-118">string</span><span class="sxs-lookup"><span data-stu-id="20bfb-118">string</span></span> | <span data-ttu-id="20bfb-119">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="20bfb-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="20bfb-120">**description**</span><span class="sxs-lookup"><span data-stu-id="20bfb-120">**description**</span></span> | <span data-ttu-id="20bfb-121">string</span><span class="sxs-lookup"><span data-stu-id="20bfb-121">string</span></span> | <span data-ttu-id="20bfb-122">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="20bfb-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20bfb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20bfb-123">JSON representation</span></span>

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
