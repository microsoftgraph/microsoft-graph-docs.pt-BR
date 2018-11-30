---
title: Tipo de recurso privacyProfile
description: Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.
ms.openlocfilehash: 5d1a8e48a2d8310f45c71fbc73485e8ec4fe8697
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006917"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="b6a68-103">Tipo de recurso privacyProfile</span><span class="sxs-lookup"><span data-stu-id="b6a68-103">privacyProfile resource type</span></span>

<span data-ttu-id="b6a68-104">Representa o perfil de privacidade de uma empresa que inclui uma URL da política de privacidade e uma pessoa de contato para tirar dúvidas sobre a política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b6a68-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="b6a68-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6a68-105">Properties</span></span>
| <span data-ttu-id="b6a68-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6a68-106">Property</span></span>   | <span data-ttu-id="b6a68-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6a68-107">Type</span></span>|<span data-ttu-id="b6a68-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a68-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6a68-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="b6a68-109">contactEmail</span></span>|<span data-ttu-id="b6a68-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6a68-110">String</span></span>| <span data-ttu-id="b6a68-111">Um endereço de email smtp válido para o contato da política de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b6a68-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="b6a68-112">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6a68-112">Not required.</span></span>|
|<span data-ttu-id="b6a68-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="b6a68-113">statementUrl</span></span>|<span data-ttu-id="b6a68-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6a68-114">String</span></span>| <span data-ttu-id="b6a68-115">Um formato de URL válido começando por http:// ou https://.</span><span class="sxs-lookup"><span data-stu-id="b6a68-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="b6a68-116">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b6a68-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="b6a68-117">A URL que direciona para a política de privacidade da empresa.</span><span class="sxs-lookup"><span data-stu-id="b6a68-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="b6a68-118">Não obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6a68-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6a68-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6a68-119">JSON representation</span></span>

<span data-ttu-id="b6a68-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b6a68-120">Here is a JSON representation of the resource</span></span>

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