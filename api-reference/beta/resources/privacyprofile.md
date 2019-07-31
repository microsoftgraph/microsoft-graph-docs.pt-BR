---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 29036620ad571566b5e3535891a9bb5ed92ad9cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008933"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="cefed-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="cefed-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cefed-104">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cefed-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="cefed-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cefed-105">Properties</span></span>
| <span data-ttu-id="cefed-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cefed-106">Property</span></span>   | <span data-ttu-id="cefed-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefed-107">Type</span></span>|<span data-ttu-id="cefed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cefed-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cefed-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="cefed-109">contactEmail</span></span>|<span data-ttu-id="cefed-110">String</span><span class="sxs-lookup"><span data-stu-id="cefed-110">String</span></span>| <span data-ttu-id="cefed-111">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cefed-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="cefed-112">Não necessário.</span><span class="sxs-lookup"><span data-stu-id="cefed-112">Not required.</span></span>|
|<span data-ttu-id="cefed-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="cefed-113">statementUrl</span></span>|<span data-ttu-id="cefed-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cefed-114">String</span></span>| <span data-ttu-id="cefed-115">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="cefed-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="cefed-116">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cefed-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="cefed-117">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="cefed-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="cefed-118">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cefed-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cefed-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cefed-119">JSON representation</span></span>

<span data-ttu-id="cefed-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cefed-120">Here is a JSON representation of the resource</span></span>

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
