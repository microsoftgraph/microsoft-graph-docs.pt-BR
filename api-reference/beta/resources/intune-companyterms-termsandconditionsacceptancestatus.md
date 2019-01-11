---
title: Tipo de recurso termsAndConditionsAcceptanceStatus
description: C) política por um determinado usuário. Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 704f1ae0f149bf91b1036713ed47279bb665d2e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880728"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="133cc-104">Tipo de recurso termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="133cc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="133cc-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="133cc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="133cc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="133cc-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="133cc-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="133cc-108">Uma entidade termsAndConditionsAcceptanceStatus representa o status de aceitação de uma política de Termos e Condições (T&C) por um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="133cc-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="133cc-109">Os usuários devem aceitar a versão mais recente dos termos para manterem o acesso ao Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="133cc-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="133cc-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="133cc-110">Methods</span></span>
|<span data-ttu-id="133cc-111">Método</span><span class="sxs-lookup"><span data-stu-id="133cc-111">Method</span></span>|<span data-ttu-id="133cc-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="133cc-112">Return Type</span></span>|<span data-ttu-id="133cc-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="133cc-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="133cc-114">Listar termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="133cc-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="133cc-115">Coleção [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)</span><span class="sxs-lookup"><span data-stu-id="133cc-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="133cc-116">Lista propriedades e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="133cc-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="133cc-117">Obter termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="133cc-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="133cc-119">Propriedades de leitura e relações do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="133cc-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="133cc-120">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="133cc-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="133cc-122">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="133cc-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="133cc-123">Excluir termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="133cc-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="133cc-124">None</span></span>|<span data-ttu-id="133cc-125">Exclui um [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="133cc-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="133cc-126">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="133cc-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="133cc-128">Atualiza as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="133cc-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="133cc-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="133cc-129">Properties</span></span>
|<span data-ttu-id="133cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="133cc-130">Property</span></span>|<span data-ttu-id="133cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="133cc-131">Type</span></span>|<span data-ttu-id="133cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="133cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="133cc-133">id</span><span class="sxs-lookup"><span data-stu-id="133cc-133">id</span></span>|<span data-ttu-id="133cc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="133cc-134">String</span></span>|<span data-ttu-id="133cc-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="133cc-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="133cc-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="133cc-136">userDisplayName</span></span>|<span data-ttu-id="133cc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="133cc-137">String</span></span>|<span data-ttu-id="133cc-138">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="133cc-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="133cc-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="133cc-139">acceptedVersion</span></span>|<span data-ttu-id="133cc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="133cc-140">Int32</span></span>|<span data-ttu-id="133cc-141">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="133cc-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="133cc-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="133cc-142">acceptedDateTime</span></span>|<span data-ttu-id="133cc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133cc-143">DateTimeOffset</span></span>|<span data-ttu-id="133cc-144">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="133cc-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="133cc-145">Relações</span><span class="sxs-lookup"><span data-stu-id="133cc-145">Relationships</span></span>
|<span data-ttu-id="133cc-146">Relação</span><span class="sxs-lookup"><span data-stu-id="133cc-146">Relationship</span></span>|<span data-ttu-id="133cc-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="133cc-147">Type</span></span>|<span data-ttu-id="133cc-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="133cc-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="133cc-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="133cc-149">termsAndConditions</span></span>|[<span data-ttu-id="133cc-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="133cc-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="133cc-151">Link de navegação para os termos e condições atribuídos.</span><span class="sxs-lookup"><span data-stu-id="133cc-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="133cc-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="133cc-152">JSON Representation</span></span>
<span data-ttu-id="133cc-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="133cc-153">Here is a JSON representation of the resource.</span></span>
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





