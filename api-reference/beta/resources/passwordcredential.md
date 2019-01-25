---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço. A propriedade **passwordCredentials** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **passwordCredential**.
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523145"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="264c0-104">tipo de recurso passwordCredential</span><span class="sxs-lookup"><span data-stu-id="264c0-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="264c0-105">Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="264c0-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="264c0-106">A propriedade **passwordCredentials** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **passwordCredential**.</span><span class="sxs-lookup"><span data-stu-id="264c0-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="264c0-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="264c0-107">JSON representation</span></span>

<span data-ttu-id="264c0-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="264c0-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="264c0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="264c0-109">Properties</span></span>
| <span data-ttu-id="264c0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="264c0-110">Property</span></span>     | <span data-ttu-id="264c0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="264c0-111">Type</span></span>   |<span data-ttu-id="264c0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="264c0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="264c0-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="264c0-113">customKeyIdentifier</span></span>|<span data-ttu-id="264c0-114">Binária</span><span class="sxs-lookup"><span data-stu-id="264c0-114">Binary</span></span>|            |
|<span data-ttu-id="264c0-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="264c0-115">endDateTime</span></span>|<span data-ttu-id="264c0-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264c0-116">DateTimeOffset</span></span>|<span data-ttu-id="264c0-117">A data e hora em que a senha expira. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="264c0-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="264c0-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="264c0-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="264c0-119">keyId</span><span class="sxs-lookup"><span data-stu-id="264c0-119">keyId</span></span>|<span data-ttu-id="264c0-120">Guid</span><span class="sxs-lookup"><span data-stu-id="264c0-120">Guid</span></span>|            |
|<span data-ttu-id="264c0-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="264c0-121">startDateTime</span></span>|<span data-ttu-id="264c0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="264c0-122">DateTimeOffset</span></span>|<span data-ttu-id="264c0-123">A data e a hora em que a senha se torna válida. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="264c0-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="264c0-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="264c0-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="264c0-125">secretText</span><span class="sxs-lookup"><span data-stu-id="264c0-125">secretText</span></span>|<span data-ttu-id="264c0-126">String</span><span class="sxs-lookup"><span data-stu-id="264c0-126">String</span></span>| <span data-ttu-id="264c0-127">As senhas devem ser 16-64 caracteres de comprimento</span><span class="sxs-lookup"><span data-stu-id="264c0-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="264c0-128">Dica</span><span class="sxs-lookup"><span data-stu-id="264c0-128">hint</span></span>|<span data-ttu-id="264c0-129">String</span><span class="sxs-lookup"><span data-stu-id="264c0-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordcredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
