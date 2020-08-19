---
title: tipo de recurso mfaDetail
description: 'Indica os detalhes de MFA de uma entrada específica. Ele inclui o método de autenticação usado para entrar e os detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: khotz
ms.openlocfilehash: f58736d890bc530239be413aec9a6920c64856ee
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809359"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="9b9c7-104">tipo de recurso mfaDetail</span><span class="sxs-lookup"><span data-stu-id="9b9c7-104">mfaDetail resource type</span></span>

<span data-ttu-id="9b9c7-105">Namespace: Microsoft. Graph indica os detalhes de MFA de uma entrada específica.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-105">Namespace: microsoft.graph Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="9b9c7-106">Ele inclui o método de autenticação usado para entrar e os detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal)</span><span class="sxs-lookup"><span data-stu-id="9b9c7-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span>



## <a name="properties"></a><span data-ttu-id="9b9c7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b9c7-107">Properties</span></span>
| <span data-ttu-id="9b9c7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b9c7-108">Property</span></span>     | <span data-ttu-id="9b9c7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b9c7-109">Type</span></span>   |<span data-ttu-id="9b9c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b9c7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b9c7-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="9b9c7-111">authDetail</span></span>|<span data-ttu-id="9b9c7-112">String</span><span class="sxs-lookup"><span data-stu-id="9b9c7-112">String</span></span>|<span data-ttu-id="9b9c7-113">Indica o detalhe de autenticação da MFA para a atividade de entrada correspondente quando a MFA necessária for "Sim".</span><span class="sxs-lookup"><span data-stu-id="9b9c7-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="9b9c7-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="9b9c7-114">authMethod</span></span>|<span data-ttu-id="9b9c7-115">String</span><span class="sxs-lookup"><span data-stu-id="9b9c7-115">String</span></span>|<span data-ttu-id="9b9c7-116">Indica os métodos de autenticação da MFA (SMS, Phone, o aplicativo autenticador são alguns dos valores) para a atividade de entrada correspondente quando o campo obrigatório do MFA é "Yes".</span><span class="sxs-lookup"><span data-stu-id="9b9c7-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b9c7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b9c7-117">JSON representation</span></span>

<span data-ttu-id="9b9c7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-118">Here is a JSON representation of the resource.</span></span>

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
