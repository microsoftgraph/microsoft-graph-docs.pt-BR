---
title: Tipo de recurso termsAndConditionsAcceptanceStatus
description: Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02dd6af7ceb216a0f53485c44b5a58eb032f6fb0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557786"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="d19dd-104">Tipo de recurso termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="d19dd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d19dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d19dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d19dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d19dd-107">Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="d19dd-107">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="d19dd-108">Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="d19dd-108">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="d19dd-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d19dd-109">Methods</span></span>
|<span data-ttu-id="d19dd-110">Método</span><span class="sxs-lookup"><span data-stu-id="d19dd-110">Method</span></span>|<span data-ttu-id="d19dd-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d19dd-111">Return Type</span></span>|<span data-ttu-id="d19dd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19dd-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d19dd-113">Listar termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="d19dd-113">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="d19dd-114">Coleção [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="d19dd-114">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="d19dd-115">Lista propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d19dd-115">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="d19dd-116">Obter termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-116">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="d19dd-117">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-117">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="d19dd-118">Propriedades de leitura e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d19dd-118">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="d19dd-119">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-119">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="d19dd-120">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-120">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="d19dd-121">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d19dd-121">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="d19dd-122">Excluir termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-122">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="d19dd-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d19dd-123">None</span></span>|<span data-ttu-id="d19dd-124">Exclui um [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d19dd-124">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="d19dd-125">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-125">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="d19dd-126">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d19dd-126">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="d19dd-127">Atualiza as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d19dd-127">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d19dd-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d19dd-128">Properties</span></span>
|<span data-ttu-id="d19dd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d19dd-129">Property</span></span>|<span data-ttu-id="d19dd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d19dd-130">Type</span></span>|<span data-ttu-id="d19dd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d19dd-132">id</span><span class="sxs-lookup"><span data-stu-id="d19dd-132">id</span></span>|<span data-ttu-id="d19dd-133">String</span><span class="sxs-lookup"><span data-stu-id="d19dd-133">String</span></span>|<span data-ttu-id="d19dd-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="d19dd-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d19dd-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d19dd-135">userDisplayName</span></span>|<span data-ttu-id="d19dd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d19dd-136">String</span></span>|<span data-ttu-id="d19dd-137">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="d19dd-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="d19dd-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="d19dd-138">acceptedVersion</span></span>|<span data-ttu-id="d19dd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d19dd-139">Int32</span></span>|<span data-ttu-id="d19dd-140">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="d19dd-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="d19dd-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="d19dd-141">acceptedDateTime</span></span>|<span data-ttu-id="d19dd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d19dd-142">DateTimeOffset</span></span>|<span data-ttu-id="d19dd-143">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="d19dd-143">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d19dd-144">Relações</span><span class="sxs-lookup"><span data-stu-id="d19dd-144">Relationships</span></span>
|<span data-ttu-id="d19dd-145">Relação</span><span class="sxs-lookup"><span data-stu-id="d19dd-145">Relationship</span></span>|<span data-ttu-id="d19dd-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="d19dd-146">Type</span></span>|<span data-ttu-id="d19dd-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19dd-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d19dd-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d19dd-148">termsAndConditions</span></span>|[<span data-ttu-id="d19dd-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d19dd-149">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="d19dd-150">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="d19dd-150">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d19dd-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d19dd-151">JSON Representation</span></span>
<span data-ttu-id="d19dd-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d19dd-152">Here is a JSON representation of the resource.</span></span>
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





