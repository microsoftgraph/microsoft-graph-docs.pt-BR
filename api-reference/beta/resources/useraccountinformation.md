---
title: tipo de recurso userAccountInformation
description: tipo de recurso userAccountInformation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0bdb0bd3856e8eaf55d19d01a8566a34810051c7
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949486"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="5775d-103">tipo de recurso userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="5775d-103">userAccountInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5775d-104">Representa informações especificamente ligadas à conta de um usuário, seja ela uma conta do Azure AD ou uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5775d-104">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="5775d-105">O identificador de entidade é definido como o GUID do Azure AD correspondente ou o CID da conta da Microsoft, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="5775d-105">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="5775d-106">Esses campos são somente leitura por meio do Microsoft Graph e devem ser editados por meio de um perfil de usuário ou por um administrador de locatários em uma experiência correspondente.</span><span class="sxs-lookup"><span data-stu-id="5775d-106">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="5775d-107">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="5775d-107">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5775d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5775d-108">Methods</span></span>

| <span data-ttu-id="5775d-109">Método</span><span class="sxs-lookup"><span data-stu-id="5775d-109">Method</span></span>                                                             | <span data-ttu-id="5775d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5775d-110">Return Type</span></span>                                         | <span data-ttu-id="5775d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5775d-111">Description</span></span>                                                         |
|:-------------------------------------------------------------------|:----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="5775d-112">Obter userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="5775d-112">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md) | [<span data-ttu-id="5775d-113">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="5775d-113">userAccountInformation</span></span>](useraccountinformation.md) | <span data-ttu-id="5775d-114">Leia as propriedades e os relacionamentos de um objeto **userAccountInformation** .</span><span class="sxs-lookup"><span data-stu-id="5775d-114">Read the properties and relationships of a **userAccountInformation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5775d-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5775d-115">Properties</span></span>

| <span data-ttu-id="5775d-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5775d-116">Property</span></span>            | <span data-ttu-id="5775d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5775d-117">Type</span></span>                       | <span data-ttu-id="5775d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5775d-118">Description</span></span>                                                                                                                              |
|:--------------------|:---------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5775d-119">ageGroup</span><span class="sxs-lookup"><span data-stu-id="5775d-119">ageGroup</span></span>             |<span data-ttu-id="5775d-120">String</span><span class="sxs-lookup"><span data-stu-id="5775d-120">String</span></span>                      | <span data-ttu-id="5775d-121">Mostra o grupo de idade do usuário.</span><span class="sxs-lookup"><span data-stu-id="5775d-121">Shows the age group of user.</span></span> <span data-ttu-id="5775d-122">Os valores `null`permitidos `minor`, `notAdult` e `adult` são gerados pelo diretório e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="5775d-122">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="5775d-123">countryCode</span><span class="sxs-lookup"><span data-stu-id="5775d-123">countryCode</span></span>          |<span data-ttu-id="5775d-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5775d-124">String</span></span>|                     | <span data-ttu-id="5775d-125">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="5775d-125">Contains the two-character country code associated with the users account.</span></span>                                                                |
|<span data-ttu-id="5775d-126">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="5775d-126">preferredLanguageTag</span></span> |[<span data-ttu-id="5775d-127">localeInfo</span><span class="sxs-lookup"><span data-stu-id="5775d-127">localeInfo</span></span>](localeinfo.md) | <span data-ttu-id="5775d-128">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="5775d-128">Contains the language the user has associated as preferred for the account.</span></span>                                                              |
|<span data-ttu-id="5775d-129">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5775d-129">userPrincipalName</span></span>    |<span data-ttu-id="5775d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5775d-130">String</span></span>                      | <span data-ttu-id="5775d-131">O nome principal do usuário (UPN) do usuário associado à conta.</span><span class="sxs-lookup"><span data-stu-id="5775d-131">The user principal name (UPN) of the user associated with the account.</span></span>                                                                   |

## <a name="relationships"></a><span data-ttu-id="5775d-132">Relações</span><span class="sxs-lookup"><span data-stu-id="5775d-132">Relationships</span></span>

<span data-ttu-id="5775d-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5775d-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5775d-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5775d-134">JSON representation</span></span>

<span data-ttu-id="5775d-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5775d-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": ""
}-->

```json
{
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {"@odata.type": "microsoft.graph.localeInfo"},
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAccountInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
