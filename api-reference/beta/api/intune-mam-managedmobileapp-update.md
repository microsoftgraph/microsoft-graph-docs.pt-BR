---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56c3646d39e90f74fa74ea47ca982417693a7691
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277481"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="c895a-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="c895a-103">Update managedMobileApp</span></span>

<span data-ttu-id="c895a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c895a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c895a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c895a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c895a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c895a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c895a-107">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c895a-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c895a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c895a-108">Prerequisites</span></span>
<span data-ttu-id="c895a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c895a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c895a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c895a-111">Permission type</span></span>|<span data-ttu-id="c895a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c895a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c895a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c895a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c895a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c895a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c895a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c895a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c895a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c895a-116">Not supported.</span></span>|
|<span data-ttu-id="c895a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c895a-117">Application</span></span>|<span data-ttu-id="c895a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c895a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c895a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c895a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c895a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c895a-120">Request headers</span></span>
|<span data-ttu-id="c895a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c895a-121">Header</span></span>|<span data-ttu-id="c895a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c895a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c895a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c895a-123">Authorization</span></span>|<span data-ttu-id="c895a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c895a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c895a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c895a-125">Accept</span></span>|<span data-ttu-id="c895a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c895a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c895a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c895a-127">Request body</span></span>
<span data-ttu-id="c895a-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c895a-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="c895a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c895a-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="c895a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c895a-130">Property</span></span>|<span data-ttu-id="c895a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c895a-131">Type</span></span>|<span data-ttu-id="c895a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c895a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c895a-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c895a-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="c895a-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c895a-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c895a-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="c895a-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="c895a-136">id</span><span class="sxs-lookup"><span data-stu-id="c895a-136">id</span></span>|<span data-ttu-id="c895a-137">String</span><span class="sxs-lookup"><span data-stu-id="c895a-137">String</span></span>|<span data-ttu-id="c895a-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c895a-138">Key of the entity.</span></span>|
|<span data-ttu-id="c895a-139">versão</span><span class="sxs-lookup"><span data-stu-id="c895a-139">version</span></span>|<span data-ttu-id="c895a-140">String</span><span class="sxs-lookup"><span data-stu-id="c895a-140">String</span></span>|<span data-ttu-id="c895a-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="c895a-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c895a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c895a-142">Response</span></span>
<span data-ttu-id="c895a-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c895a-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c895a-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c895a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c895a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c895a-145">Request</span></span>
<span data-ttu-id="c895a-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c895a-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="c895a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c895a-147">Response</span></span>
<span data-ttu-id="c895a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c895a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




