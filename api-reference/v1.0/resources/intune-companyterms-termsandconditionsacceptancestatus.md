---
title: Tipo de recurso termsAndConditionsAcceptanceStatus
description: C) política por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.
ms.openlocfilehash: 331d80481624caa0083414e7b3a8f12ba414991f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006236"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="ebcc2-104">Tipo de recurso termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="ebcc2-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebcc2-106">Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="ebcc2-107">Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="ebcc2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ebcc2-108">Methods</span></span>
|<span data-ttu-id="ebcc2-109">Método</span><span class="sxs-lookup"><span data-stu-id="ebcc2-109">Method</span></span>|<span data-ttu-id="ebcc2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ebcc2-110">Return Type</span></span>|<span data-ttu-id="ebcc2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcc2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebcc2-112">Listar termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="ebcc2-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="ebcc2-113">Coleção [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="ebcc2-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="ebcc2-114">Lista propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ebcc2-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="ebcc2-115">Obter termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="ebcc2-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="ebcc2-117">Propriedades de leitura e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ebcc2-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="ebcc2-118">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="ebcc2-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="ebcc2-120">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ebcc2-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="ebcc2-121">Excluir termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="ebcc2-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ebcc2-122">None</span></span>|<span data-ttu-id="ebcc2-123">Exclui um [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ebcc2-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="ebcc2-124">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="ebcc2-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ebcc2-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="ebcc2-126">Atualiza as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ebcc2-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebcc2-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebcc2-127">Properties</span></span>
|<span data-ttu-id="ebcc2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebcc2-128">Property</span></span>|<span data-ttu-id="ebcc2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebcc2-129">Type</span></span>|<span data-ttu-id="ebcc2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcc2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebcc2-131">id</span><span class="sxs-lookup"><span data-stu-id="ebcc2-131">id</span></span>|<span data-ttu-id="ebcc2-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebcc2-132">String</span></span>|<span data-ttu-id="ebcc2-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="ebcc2-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ebcc2-134">userDisplayName</span></span>|<span data-ttu-id="ebcc2-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebcc2-135">String</span></span>|<span data-ttu-id="ebcc2-136">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="ebcc2-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="ebcc2-137">acceptedVersion</span></span>|<span data-ttu-id="ebcc2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ebcc2-138">Int32</span></span>|<span data-ttu-id="ebcc2-139">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="ebcc2-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebcc2-140">acceptedDateTime</span></span>|<span data-ttu-id="ebcc2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebcc2-141">DateTimeOffset</span></span>|<span data-ttu-id="ebcc2-142">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebcc2-143">Relações</span><span class="sxs-lookup"><span data-stu-id="ebcc2-143">Relationships</span></span>
|<span data-ttu-id="ebcc2-144">Relação</span><span class="sxs-lookup"><span data-stu-id="ebcc2-144">Relationship</span></span>|<span data-ttu-id="ebcc2-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebcc2-145">Type</span></span>|<span data-ttu-id="ebcc2-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcc2-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebcc2-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ebcc2-147">termsAndConditions</span></span>|[<span data-ttu-id="ebcc2-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ebcc2-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="ebcc2-149">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebcc2-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebcc2-150">JSON Representation</span></span>
<span data-ttu-id="ebcc2-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebcc2-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



