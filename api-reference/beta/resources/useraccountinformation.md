---
title: tipo de recurso userAccountInformation
description: tipo de recurso userAccountInformation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b2993348b19cd0f55cbb7d26369276ea97006960
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846076"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="9473f-103">tipo de recurso userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="9473f-103">userAccountInformation resource type</span></span>

<span data-ttu-id="9473f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9473f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9473f-105">Representa informações especificamente ligadas à conta de um usuário, seja ela uma conta do Azure AD ou uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9473f-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="9473f-106">O identificador de entidade é definido como o GUID do Azure AD correspondente ou o CID da conta da Microsoft, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="9473f-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="9473f-107">Esses campos são somente leitura por meio do Microsoft Graph e devem ser editados por meio de um perfil de usuário ou por um administrador de locatários em uma experiência correspondente.</span><span class="sxs-lookup"><span data-stu-id="9473f-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="9473f-108">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="9473f-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9473f-109">Methods</span><span class="sxs-lookup"><span data-stu-id="9473f-109">Methods</span></span>

| <span data-ttu-id="9473f-110">Método</span><span class="sxs-lookup"><span data-stu-id="9473f-110">Method</span></span>                                                             | <span data-ttu-id="9473f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9473f-111">Return Type</span></span>                                         | <span data-ttu-id="9473f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9473f-112">Description</span></span>                                                                   |
|:-------------------------------------------------------------------|:----------------------------------------------------|:------------------------------------------------------------------------------|
| [<span data-ttu-id="9473f-113">Obter userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="9473f-113">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md) | [<span data-ttu-id="9473f-114">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="9473f-114">userAccountInformation</span></span>](useraccountinformation.md) | <span data-ttu-id="9473f-115">Leia as propriedades e os relacionamentos de um objeto **userAccountInformation** .</span><span class="sxs-lookup"><span data-stu-id="9473f-115">Read the properties and relationships of a **userAccountInformation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9473f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9473f-116">Properties</span></span>

| <span data-ttu-id="9473f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9473f-117">Property</span></span>             | <span data-ttu-id="9473f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9473f-118">Type</span></span>                        | <span data-ttu-id="9473f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9473f-119">Description</span></span>                                                                                                                               |
|:---------------------|:----------------------------|:------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9473f-120">ageGroup</span><span class="sxs-lookup"><span data-stu-id="9473f-120">ageGroup</span></span>             | <span data-ttu-id="9473f-121">String</span><span class="sxs-lookup"><span data-stu-id="9473f-121">String</span></span>                      | <span data-ttu-id="9473f-122">Mostra o grupo de idade do usuário.</span><span class="sxs-lookup"><span data-stu-id="9473f-122">Shows the age group of user.</span></span> <span data-ttu-id="9473f-123">Os valores `null` permitidos `minor` , `notAdult` e `adult` são gerados pelo diretório e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="9473f-123">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span> |
| <span data-ttu-id="9473f-124">countryCode</span><span class="sxs-lookup"><span data-stu-id="9473f-124">countryCode</span></span>          | <span data-ttu-id="9473f-125">String</span><span class="sxs-lookup"><span data-stu-id="9473f-125">String</span></span>                      | <span data-ttu-id="9473f-126">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="9473f-126">Contains the two-character country code associated with the users account.</span></span>                                                                |
| <span data-ttu-id="9473f-127">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="9473f-127">preferredLanguageTag</span></span> | [<span data-ttu-id="9473f-128">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9473f-128">localeInfo</span></span>](localeinfo.md) | <span data-ttu-id="9473f-129">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="9473f-129">Contains the language the user has associated as preferred for the account.</span></span>                                                               |
| <span data-ttu-id="9473f-130">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9473f-130">userPrincipalName</span></span>    | <span data-ttu-id="9473f-131">String</span><span class="sxs-lookup"><span data-stu-id="9473f-131">String</span></span>                      | <span data-ttu-id="9473f-132">O nome principal do usuário (UPN) do usuário associado à conta.</span><span class="sxs-lookup"><span data-stu-id="9473f-132">The user principal name (UPN) of the user associated with the account.</span></span>                                                                    |

## <a name="relationships"></a><span data-ttu-id="9473f-133">Relações</span><span class="sxs-lookup"><span data-stu-id="9473f-133">Relationships</span></span>

<span data-ttu-id="9473f-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9473f-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9473f-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9473f-135">JSON representation</span></span>

<span data-ttu-id="9473f-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9473f-136">The following is a JSON representation of the resource.</span></span>

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
