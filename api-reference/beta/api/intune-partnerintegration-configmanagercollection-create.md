---
title: Criar configManagerCollection
description: Criar um novo objeto configManagerCollection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a16a878140e233e44960d842687f05f0c2c7a79e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301451"
---
# <a name="create-configmanagercollection"></a><span data-ttu-id="45837-103">Criar configManagerCollection</span><span class="sxs-lookup"><span data-stu-id="45837-103">Create configManagerCollection</span></span>

<span data-ttu-id="45837-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45837-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45837-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45837-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45837-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45837-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45837-107">Criar um novo objeto [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) .</span><span class="sxs-lookup"><span data-stu-id="45837-107">Create a new [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45837-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45837-108">Prerequisites</span></span>
<span data-ttu-id="45837-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45837-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45837-111">Permission type</span></span>|<span data-ttu-id="45837-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45837-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45837-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45837-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45837-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45837-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45837-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45837-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45837-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45837-116">Not supported.</span></span>|
|<span data-ttu-id="45837-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45837-117">Application</span></span>|<span data-ttu-id="45837-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45837-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45837-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45837-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="45837-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45837-120">Request headers</span></span>
|<span data-ttu-id="45837-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45837-121">Header</span></span>|<span data-ttu-id="45837-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45837-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45837-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45837-123">Authorization</span></span>|<span data-ttu-id="45837-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45837-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45837-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45837-125">Accept</span></span>|<span data-ttu-id="45837-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45837-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45837-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45837-127">Request body</span></span>
<span data-ttu-id="45837-128">No corpo da solicitação, forneça uma representação JSON do objeto configManagerCollection.</span><span class="sxs-lookup"><span data-stu-id="45837-128">In the request body, supply a JSON representation for the configManagerCollection object.</span></span>

<span data-ttu-id="45837-129">A tabela a seguir mostra as propriedades que são necessárias ao criar configManagerCollection.</span><span class="sxs-lookup"><span data-stu-id="45837-129">The following table shows the properties that are required when you create the configManagerCollection.</span></span>

|<span data-ttu-id="45837-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45837-130">Property</span></span>|<span data-ttu-id="45837-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45837-131">Type</span></span>|<span data-ttu-id="45837-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45837-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45837-133">id</span><span class="sxs-lookup"><span data-stu-id="45837-133">id</span></span>|<span data-ttu-id="45837-134">String</span><span class="sxs-lookup"><span data-stu-id="45837-134">String</span></span>|<span data-ttu-id="45837-135">A chave da coleção Configmanager.</span><span class="sxs-lookup"><span data-stu-id="45837-135">The key for the ConfigManager Collection.</span></span>|
|<span data-ttu-id="45837-136">displayName</span><span class="sxs-lookup"><span data-stu-id="45837-136">displayName</span></span>|<span data-ttu-id="45837-137">String</span><span class="sxs-lookup"><span data-stu-id="45837-137">String</span></span>|<span data-ttu-id="45837-138">O DisplayName.</span><span class="sxs-lookup"><span data-stu-id="45837-138">The DisplayName.</span></span>|
|<span data-ttu-id="45837-139">collectionIdentifier</span><span class="sxs-lookup"><span data-stu-id="45837-139">collectionIdentifier</span></span>|<span data-ttu-id="45837-140">String</span><span class="sxs-lookup"><span data-stu-id="45837-140">String</span></span>|<span data-ttu-id="45837-141">O identificador de coleção no SCCM.</span><span class="sxs-lookup"><span data-stu-id="45837-141">The collection identifier in SCCM.</span></span>|
|<span data-ttu-id="45837-142">HierarchyName</span><span class="sxs-lookup"><span data-stu-id="45837-142">hierarchyName</span></span>|<span data-ttu-id="45837-143">String</span><span class="sxs-lookup"><span data-stu-id="45837-143">String</span></span>|<span data-ttu-id="45837-144">O HierarchyName.</span><span class="sxs-lookup"><span data-stu-id="45837-144">The HierarchyName.</span></span>|
|<span data-ttu-id="45837-145">hierarchyIdentifier</span><span class="sxs-lookup"><span data-stu-id="45837-145">hierarchyIdentifier</span></span>|<span data-ttu-id="45837-146">String</span><span class="sxs-lookup"><span data-stu-id="45837-146">String</span></span>|<span data-ttu-id="45837-147">O identificador de hierarquia.</span><span class="sxs-lookup"><span data-stu-id="45837-147">The Hierarchy Identifier.</span></span>|
|<span data-ttu-id="45837-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45837-148">createdDateTime</span></span>|<span data-ttu-id="45837-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45837-149">DateTimeOffset</span></span>|<span data-ttu-id="45837-150">A data de criação.</span><span class="sxs-lookup"><span data-stu-id="45837-150">The created date.</span></span>|
|<span data-ttu-id="45837-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45837-151">lastModifiedDateTime</span></span>|<span data-ttu-id="45837-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45837-152">DateTimeOffset</span></span>|<span data-ttu-id="45837-153">A data da última modificação.</span><span class="sxs-lookup"><span data-stu-id="45837-153">The last modified date.</span></span>|



## <a name="response"></a><span data-ttu-id="45837-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="45837-154">Response</span></span>
<span data-ttu-id="45837-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45837-155">If successful, this method returns a `201 Created` response code and a [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45837-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45837-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="45837-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45837-157">Request</span></span>
<span data-ttu-id="45837-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45837-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value"
}
```

### <a name="response"></a><span data-ttu-id="45837-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="45837-159">Response</span></span>
<span data-ttu-id="45837-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45837-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 435

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




