---
title: Tipo de recurso mfaDetail
description: 'Indica detalhes do MFA para uma assinatura específica. Ele inclui o método de autenticação usado para entrar, bem como detalhes de autenticação (por exemplo: Telefone, SMS ou caixa postal) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b3cd2392b9591cfb5465f2f269db547cd37754ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759794"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="a0940-104">Tipo de recurso mfaDetail</span><span class="sxs-lookup"><span data-stu-id="a0940-104">mfaDetail resource type</span></span>

<span data-ttu-id="a0940-105">Namespace: microsoft.graph Indica detalhes de MFA para uma conexão específica.</span><span class="sxs-lookup"><span data-stu-id="a0940-105">Namespace: microsoft.graph Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="a0940-106">Ele inclui o método de autenticação usado para entrar, bem como detalhes de autenticação (por exemplo: Telefone, SMS ou caixa postal)</span><span class="sxs-lookup"><span data-stu-id="a0940-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span>



## <a name="properties"></a><span data-ttu-id="a0940-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0940-107">Properties</span></span>
| <span data-ttu-id="a0940-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0940-108">Property</span></span>     | <span data-ttu-id="a0940-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0940-109">Type</span></span>   |<span data-ttu-id="a0940-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0940-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0940-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="a0940-111">authDetail</span></span>|<span data-ttu-id="a0940-112">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a0940-112">String</span></span>|<span data-ttu-id="a0940-113">Indica o detalhe de auth MFA para a atividade de Login correspondente quando o MFA Obrigatório é "Sim".</span><span class="sxs-lookup"><span data-stu-id="a0940-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="a0940-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="a0940-114">authMethod</span></span>|<span data-ttu-id="a0940-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a0940-115">String</span></span>|<span data-ttu-id="a0940-116">Indica que os métodos MFA Auth (SMS, Telefone, Aplicativo Autenticador são parte do valor) para a atividade de login correspondente quando o campo MFA Obrigatório for "Sim".</span><span class="sxs-lookup"><span data-stu-id="a0940-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0940-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0940-117">JSON representation</span></span>

<span data-ttu-id="a0940-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0940-118">Here is a JSON representation of the resource.</span></span>

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


