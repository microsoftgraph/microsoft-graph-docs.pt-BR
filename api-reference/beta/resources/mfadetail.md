---
title: tipo de recurso de mfaDetail
description: 'Indica os detalhes MFA para uma entrada específica. Inclui o método de autenticação usado para fazer o login, bem como detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) '
ms.openlocfilehash: a377c8648ebc8a6e3eb10fb6b0b87df066f8f2cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036417"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="fc804-104">tipo de recurso de mfaDetail</span><span class="sxs-lookup"><span data-stu-id="fc804-104">mfaDetail resource type</span></span>
<span data-ttu-id="fc804-105">Indica os detalhes MFA para uma entrada específica.</span><span class="sxs-lookup"><span data-stu-id="fc804-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="fc804-106">Inclui o método de autenticação usado para fazer o login, bem como detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal)</span><span class="sxs-lookup"><span data-stu-id="fc804-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="fc804-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc804-107">Properties</span></span>
| <span data-ttu-id="fc804-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc804-108">Property</span></span>     | <span data-ttu-id="fc804-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc804-109">Type</span></span>   |<span data-ttu-id="fc804-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc804-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc804-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="fc804-111">authDetail</span></span>|<span data-ttu-id="fc804-112">String</span><span class="sxs-lookup"><span data-stu-id="fc804-112">String</span></span>|<span data-ttu-id="fc804-113">Indica o detalhe de autenticação MFA da atividade de entrada correspondentes quando o MFA necessário é "Yes".</span><span class="sxs-lookup"><span data-stu-id="fc804-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="fc804-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="fc804-114">authMethod</span></span>|<span data-ttu-id="fc804-115">String</span><span class="sxs-lookup"><span data-stu-id="fc804-115">String</span></span>|<span data-ttu-id="fc804-116">Indica os métodos de autenticação MFA (SMS, telefone, autenticador App são alguns do valor) para a atividade de entrada correspondente quando o campo MFA necessário é "Yes".</span><span class="sxs-lookup"><span data-stu-id="fc804-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc804-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc804-117">JSON representation</span></span>

<span data-ttu-id="fc804-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc804-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->