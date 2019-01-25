---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510117"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="f0721-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f0721-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0721-104">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f0721-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="f0721-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0721-105">Properties</span></span>
| <span data-ttu-id="f0721-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0721-106">Property</span></span>   | <span data-ttu-id="f0721-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0721-107">Type</span></span>|<span data-ttu-id="f0721-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0721-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0721-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="f0721-109">contactEmail</span></span>|<span data-ttu-id="f0721-110">String</span><span class="sxs-lookup"><span data-stu-id="f0721-110">String</span></span>| <span data-ttu-id="f0721-111">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f0721-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="f0721-112">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0721-112">Not required.</span></span>|
|<span data-ttu-id="f0721-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="f0721-113">statementUrl</span></span>|<span data-ttu-id="f0721-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0721-114">String</span></span>| <span data-ttu-id="f0721-115">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="f0721-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="f0721-116">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="f0721-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="f0721-117">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0721-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="f0721-118">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0721-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0721-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0721-119">JSON representation</span></span>

<span data-ttu-id="f0721-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f0721-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
