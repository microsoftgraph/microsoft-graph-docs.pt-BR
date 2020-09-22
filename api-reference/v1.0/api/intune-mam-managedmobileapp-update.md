---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61e9d320a77eab0dbe041a6b6e1dd6b96ed60422
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015831"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="af188-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="af188-103">Update managedMobileApp</span></span>

<span data-ttu-id="af188-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af188-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af188-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af188-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af188-106">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af188-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af188-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af188-107">Prerequisites</span></span>
<span data-ttu-id="af188-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af188-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af188-110">Permission type</span></span>|<span data-ttu-id="af188-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af188-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af188-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af188-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af188-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af188-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af188-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af188-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af188-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af188-115">Not supported.</span></span>|
|<span data-ttu-id="af188-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af188-116">Application</span></span>|<span data-ttu-id="af188-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af188-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af188-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af188-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="af188-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af188-119">Request headers</span></span>
|<span data-ttu-id="af188-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af188-120">Header</span></span>|<span data-ttu-id="af188-121">Valor</span><span class="sxs-lookup"><span data-stu-id="af188-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af188-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af188-122">Authorization</span></span>|<span data-ttu-id="af188-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af188-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af188-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af188-124">Accept</span></span>|<span data-ttu-id="af188-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af188-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af188-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af188-126">Request body</span></span>
<span data-ttu-id="af188-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af188-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="af188-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af188-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="af188-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af188-129">Property</span></span>|<span data-ttu-id="af188-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="af188-130">Type</span></span>|<span data-ttu-id="af188-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="af188-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af188-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="af188-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="af188-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="af188-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="af188-134">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="af188-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="af188-135">id</span><span class="sxs-lookup"><span data-stu-id="af188-135">id</span></span>|<span data-ttu-id="af188-136">String</span><span class="sxs-lookup"><span data-stu-id="af188-136">String</span></span>|<span data-ttu-id="af188-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="af188-137">Key of the entity.</span></span>|
|<span data-ttu-id="af188-138">versão</span><span class="sxs-lookup"><span data-stu-id="af188-138">version</span></span>|<span data-ttu-id="af188-139">String</span><span class="sxs-lookup"><span data-stu-id="af188-139">String</span></span>|<span data-ttu-id="af188-140">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="af188-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="af188-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="af188-141">Response</span></span>
<span data-ttu-id="af188-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af188-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af188-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af188-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="af188-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af188-144">Request</span></span>
<span data-ttu-id="af188-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af188-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="af188-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="af188-146">Response</span></span>
<span data-ttu-id="af188-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af188-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```









