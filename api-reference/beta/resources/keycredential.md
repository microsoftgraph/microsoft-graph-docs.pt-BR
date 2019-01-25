---
title: tipo de recurso de keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A propriedade **keyCredentials** das entidades que aplicativo e servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519049"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="86cc6-104">tipo de recurso de keyCredential</span><span class="sxs-lookup"><span data-stu-id="86cc6-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86cc6-105">Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="86cc6-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="86cc6-106">A propriedade **keyCredentials** das entidades que [aplicativo](application.md) e [servicePrincipal](serviceprincipal.md) é uma coleção de **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="86cc6-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="86cc6-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86cc6-107">JSON representation</span></span>

<span data-ttu-id="86cc6-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="86cc6-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="86cc6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86cc6-109">Properties</span></span>
| <span data-ttu-id="86cc6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86cc6-110">Property</span></span>     | <span data-ttu-id="86cc6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="86cc6-111">Type</span></span>   |<span data-ttu-id="86cc6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="86cc6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86cc6-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="86cc6-113">customKeyIdentifier</span></span>|<span data-ttu-id="86cc6-114">Binária</span><span class="sxs-lookup"><span data-stu-id="86cc6-114">Binary</span></span>| <span data-ttu-id="86cc6-115">Identificador de chave personalizado</span><span class="sxs-lookup"><span data-stu-id="86cc6-115">Custom key identifier</span></span> |
|<span data-ttu-id="86cc6-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="86cc6-116">endDateTime</span></span>|<span data-ttu-id="86cc6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86cc6-117">DateTimeOffset</span></span>|<span data-ttu-id="86cc6-118">A data e hora em que a credencial de expiração. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="86cc6-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86cc6-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="86cc6-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="86cc6-120">keyId</span><span class="sxs-lookup"><span data-stu-id="86cc6-120">keyId</span></span>|<span data-ttu-id="86cc6-121">Guid</span><span class="sxs-lookup"><span data-stu-id="86cc6-121">Guid</span></span>|<span data-ttu-id="86cc6-122">O identificador exclusivo (GUID) para a chave.</span><span class="sxs-lookup"><span data-stu-id="86cc6-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="86cc6-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="86cc6-123">startDateTime</span></span>|<span data-ttu-id="86cc6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86cc6-124">DateTimeOffset</span></span>|<span data-ttu-id="86cc6-125">A data e hora em que a credencial torna-se válido. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="86cc6-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86cc6-126">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="86cc6-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="86cc6-127">type</span><span class="sxs-lookup"><span data-stu-id="86cc6-127">type</span></span>|<span data-ttu-id="86cc6-128">String</span><span class="sxs-lookup"><span data-stu-id="86cc6-128">String</span></span>|<span data-ttu-id="86cc6-129">O tipo de credencial de chave; Por exemplo, "Simétrico".</span><span class="sxs-lookup"><span data-stu-id="86cc6-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="86cc6-130">Uso</span><span class="sxs-lookup"><span data-stu-id="86cc6-130">usage</span></span>|<span data-ttu-id="86cc6-131">String</span><span class="sxs-lookup"><span data-stu-id="86cc6-131">String</span></span>|<span data-ttu-id="86cc6-132">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; Por exemplo, "Verificar".</span><span class="sxs-lookup"><span data-stu-id="86cc6-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="86cc6-133">chave</span><span class="sxs-lookup"><span data-stu-id="86cc6-133">key</span></span>|<span data-ttu-id="86cc6-134">Binário</span><span class="sxs-lookup"><span data-stu-id="86cc6-134">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keycredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
