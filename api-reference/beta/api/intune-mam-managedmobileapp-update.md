---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5350cba84f737a617bee608ea24fcf105126a47
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157845"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="17735-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="17735-103">Update managedMobileApp</span></span>

<span data-ttu-id="17735-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17735-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17735-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17735-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17735-107">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17735-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17735-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17735-108">Prerequisites</span></span>
<span data-ttu-id="17735-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17735-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17735-111">Permission type</span></span>|<span data-ttu-id="17735-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17735-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17735-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17735-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17735-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17735-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17735-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17735-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17735-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17735-116">Not supported.</span></span>|
|<span data-ttu-id="17735-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17735-117">Application</span></span>|<span data-ttu-id="17735-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17735-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17735-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17735-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="17735-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17735-120">Request headers</span></span>
|<span data-ttu-id="17735-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17735-121">Header</span></span>|<span data-ttu-id="17735-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17735-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17735-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17735-123">Authorization</span></span>|<span data-ttu-id="17735-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17735-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17735-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17735-125">Accept</span></span>|<span data-ttu-id="17735-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17735-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17735-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17735-127">Request body</span></span>
<span data-ttu-id="17735-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17735-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="17735-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17735-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="17735-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17735-130">Property</span></span>|<span data-ttu-id="17735-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17735-131">Type</span></span>|<span data-ttu-id="17735-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17735-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17735-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="17735-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="17735-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="17735-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="17735-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="17735-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="17735-136">id</span><span class="sxs-lookup"><span data-stu-id="17735-136">id</span></span>|<span data-ttu-id="17735-137">String</span><span class="sxs-lookup"><span data-stu-id="17735-137">String</span></span>|<span data-ttu-id="17735-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17735-138">Key of the entity.</span></span>|
|<span data-ttu-id="17735-139">versão</span><span class="sxs-lookup"><span data-stu-id="17735-139">version</span></span>|<span data-ttu-id="17735-140">String</span><span class="sxs-lookup"><span data-stu-id="17735-140">String</span></span>|<span data-ttu-id="17735-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="17735-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="17735-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="17735-142">Response</span></span>
<span data-ttu-id="17735-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17735-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17735-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17735-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="17735-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17735-145">Request</span></span>
<span data-ttu-id="17735-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17735-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "Windows App Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="17735-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="17735-147">Response</span></span>
<span data-ttu-id="17735-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17735-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "Windows App Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




