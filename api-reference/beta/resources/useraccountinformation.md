---
title: tipo de recurso userAccountInformation
description: tipo de recurso userAccountInformation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a633b6de9269b67fcf26dea035438a3494c4515c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812741"
---
# <a name="useraccountinformation-resource-type"></a><span data-ttu-id="84b8e-103">tipo de recurso userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-103">userAccountInformation resource type</span></span>

<span data-ttu-id="84b8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84b8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84b8e-105">Representa informações especificamente ligadas à conta de um usuário, seja ela uma conta do Azure AD ou uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="84b8e-105">Represents information specifically tied to a user's account, whether that is as an Azure AD account or Microsoft account.</span></span> <span data-ttu-id="84b8e-106">O identificador de entidade é definido como o GUID do Azure AD correspondente ou o CID da conta da Microsoft, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="84b8e-106">The entity identifier is set to the corresponding Azure AD guid or Microsoft Account CID respectively.</span></span> <span data-ttu-id="84b8e-107">Esses campos são somente leitura por meio do Microsoft Graph e devem ser editados por meio de um perfil de usuário ou por um administrador de locatários em uma experiência correspondente.</span><span class="sxs-lookup"><span data-stu-id="84b8e-107">These fields are read-only through Microsoft Graph and must be edited through a users profile or by a Tenant Administrator on a corresponding experience.</span></span>

<span data-ttu-id="84b8e-108">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-108">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="84b8e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="84b8e-109">Methods</span></span>

|<span data-ttu-id="84b8e-110">Método</span><span class="sxs-lookup"><span data-stu-id="84b8e-110">Method</span></span>|<span data-ttu-id="84b8e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="84b8e-111">Return type</span></span>|<span data-ttu-id="84b8e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b8e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84b8e-113">Listar contas</span><span class="sxs-lookup"><span data-stu-id="84b8e-113">List accounts</span></span>](../api/profile-list-accounts.md)|<span data-ttu-id="84b8e-114">coleção [userAccountInformation](../resources/useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="84b8e-114">[userAccountInformation](../resources/useraccountinformation.md) collection</span></span>|<span data-ttu-id="84b8e-115">Obtenha os recursos userAccountInformation da propriedade de navegação Account.</span><span class="sxs-lookup"><span data-stu-id="84b8e-115">Get the userAccountInformation resources from the account navigation property.</span></span>|
|[<span data-ttu-id="84b8e-116">Criar userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-116">Create userAccountInformation</span></span>](../api/profile-post-accounts.md)|[<span data-ttu-id="84b8e-117">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-117">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="84b8e-118">Criar um novo objeto userAccountInformation.</span><span class="sxs-lookup"><span data-stu-id="84b8e-118">Create a new userAccountInformation object.</span></span>|
|[<span data-ttu-id="84b8e-119">Obter userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-119">Get userAccountInformation</span></span>](../api/useraccountinformation-get.md)|[<span data-ttu-id="84b8e-120">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-120">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="84b8e-121">Leia as propriedades e os relacionamentos de um objeto [userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="84b8e-121">Read the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="84b8e-122">Atualizar userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-122">Update userAccountInformation</span></span>](../api/useraccountinformation-update.md)|[<span data-ttu-id="84b8e-123">userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-123">userAccountInformation</span></span>](../resources/useraccountinformation.md)|<span data-ttu-id="84b8e-124">Atualiza as propriedades de um objeto [userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="84b8e-124">Update the properties of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|
|[<span data-ttu-id="84b8e-125">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="84b8e-125">Delete userAccountInformation</span></span>](../api/useraccountinformation-delete.md)|<span data-ttu-id="84b8e-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84b8e-126">None</span></span>|<span data-ttu-id="84b8e-127">Exclui um objeto [userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="84b8e-127">Deletes a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84b8e-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84b8e-128">Properties</span></span>

|<span data-ttu-id="84b8e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84b8e-129">Property</span></span>|<span data-ttu-id="84b8e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="84b8e-130">Type</span></span>|<span data-ttu-id="84b8e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84b8e-132">ageGroup</span><span class="sxs-lookup"><span data-stu-id="84b8e-132">ageGroup</span></span>|<span data-ttu-id="84b8e-133">String</span><span class="sxs-lookup"><span data-stu-id="84b8e-133">String</span></span>|<span data-ttu-id="84b8e-134">Mostra o grupo de idade do usuário.</span><span class="sxs-lookup"><span data-stu-id="84b8e-134">Shows the age group of user.</span></span> <span data-ttu-id="84b8e-135">Os valores `null` permitidos `minor` , `notAdult` e `adult` são gerados pelo diretório e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="84b8e-135">Allowed values `null`, `minor`, `notAdult` and `adult` are generated by the directory and cannot be changed.</span></span>|
|<span data-ttu-id="84b8e-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="84b8e-136">allowedAudiences</span></span>|<span data-ttu-id="84b8e-137">String</span><span class="sxs-lookup"><span data-stu-id="84b8e-137">String</span></span>|<span data-ttu-id="84b8e-138">As audiências que podem ver os valores contidos na entidade.</span><span class="sxs-lookup"><span data-stu-id="84b8e-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="84b8e-139">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="84b8e-140">Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="84b8e-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="84b8e-141">countryCode</span><span class="sxs-lookup"><span data-stu-id="84b8e-141">countryCode</span></span>|<span data-ttu-id="84b8e-142">String</span><span class="sxs-lookup"><span data-stu-id="84b8e-142">String</span></span>|<span data-ttu-id="84b8e-143">Contém o código de país de dois caracteres associado à conta de usuários.</span><span class="sxs-lookup"><span data-stu-id="84b8e-143">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="84b8e-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="84b8e-144">createdBy</span></span>|[<span data-ttu-id="84b8e-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="84b8e-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="84b8e-146">Fornece o identificador do usuário e/ou aplicativo que criou a entidade.</span><span class="sxs-lookup"><span data-stu-id="84b8e-146">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="84b8e-147">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="84b8e-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84b8e-148">createdDateTime</span></span>|<span data-ttu-id="84b8e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84b8e-149">DateTimeOffset</span></span>|<span data-ttu-id="84b8e-150">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="84b8e-150">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="84b8e-151">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="84b8e-152">id</span><span class="sxs-lookup"><span data-stu-id="84b8e-152">id</span></span>|<span data-ttu-id="84b8e-153">String</span><span class="sxs-lookup"><span data-stu-id="84b8e-153">String</span></span>|<span data-ttu-id="84b8e-154">Identificador usado para o endereçamento individual da entidade.</span><span class="sxs-lookup"><span data-stu-id="84b8e-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="84b8e-155">Herdado da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="84b8e-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="84b8e-156">fracassa</span><span class="sxs-lookup"><span data-stu-id="84b8e-156">inference</span></span>|[<span data-ttu-id="84b8e-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="84b8e-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="84b8e-158">Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação.</span><span class="sxs-lookup"><span data-stu-id="84b8e-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="84b8e-159">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="84b8e-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="84b8e-160">lastModifiedBy</span></span>|[<span data-ttu-id="84b8e-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="84b8e-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="84b8e-162">Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez.</span><span class="sxs-lookup"><span data-stu-id="84b8e-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="84b8e-163">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="84b8e-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84b8e-164">lastModifiedDateTime</span></span>|<span data-ttu-id="84b8e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84b8e-165">DateTimeOffset</span></span>|<span data-ttu-id="84b8e-166">Fornece o dateTimeOffset para quando a entidade foi criada.</span><span class="sxs-lookup"><span data-stu-id="84b8e-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="84b8e-167">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="84b8e-168">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="84b8e-168">preferredLanguageTag</span></span>|[<span data-ttu-id="84b8e-169">localeInfo</span><span class="sxs-lookup"><span data-stu-id="84b8e-169">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="84b8e-170">Contém o idioma que o usuário associou como preferencial para a conta.</span><span class="sxs-lookup"><span data-stu-id="84b8e-170">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="84b8e-171">source</span><span class="sxs-lookup"><span data-stu-id="84b8e-171">source</span></span>|[<span data-ttu-id="84b8e-172">personDataSource</span><span class="sxs-lookup"><span data-stu-id="84b8e-172">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="84b8e-173">Onde os valores são originados se forem sincronizados a partir de outro serviço.</span><span class="sxs-lookup"><span data-stu-id="84b8e-173">Where the values originated if synced from another service.</span></span> <span data-ttu-id="84b8e-174">Herdado de [MyFace](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="84b8e-174">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="84b8e-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84b8e-175">userPrincipalName</span></span>|<span data-ttu-id="84b8e-176">String</span><span class="sxs-lookup"><span data-stu-id="84b8e-176">String</span></span>|<span data-ttu-id="84b8e-177">O nome principal do usuário (UPN) do usuário associado à conta.</span><span class="sxs-lookup"><span data-stu-id="84b8e-177">The user principal name (UPN) of the user associated with the account.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="84b8e-178">Relações</span><span class="sxs-lookup"><span data-stu-id="84b8e-178">Relationships</span></span>
<span data-ttu-id="84b8e-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84b8e-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84b8e-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84b8e-180">JSON representation</span></span>
<span data-ttu-id="84b8e-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84b8e-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```
