---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
ms.openlocfilehash: d1d7593e5b0f0ef9d4ac36f902ec244e93fd51c1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344197"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="c23b8-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="c23b8-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c23b8-104">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c23b8-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="c23b8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c23b8-105">Properties</span></span>
| <span data-ttu-id="c23b8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c23b8-106">Property</span></span>   | <span data-ttu-id="c23b8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c23b8-107">Type</span></span>|<span data-ttu-id="c23b8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c23b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c23b8-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="c23b8-109">contactEmail</span></span>|<span data-ttu-id="c23b8-110">String</span><span class="sxs-lookup"><span data-stu-id="c23b8-110">String</span></span>| <span data-ttu-id="c23b8-111">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c23b8-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="c23b8-112">Não necessário.</span><span class="sxs-lookup"><span data-stu-id="c23b8-112">Not required.</span></span>|
|<span data-ttu-id="c23b8-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="c23b8-113">statementUrl</span></span>|<span data-ttu-id="c23b8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c23b8-114">String</span></span>| <span data-ttu-id="c23b8-115">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="c23b8-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="c23b8-116">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c23b8-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="c23b8-117">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="c23b8-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="c23b8-118">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c23b8-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c23b8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c23b8-119">JSON representation</span></span>

<span data-ttu-id="c23b8-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c23b8-120">Here is a JSON representation of the resource</span></span>

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
