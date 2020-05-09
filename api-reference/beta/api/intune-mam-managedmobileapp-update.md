---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 268e0984dc062ecb73a412501865e1483255739e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178182"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="5bfc9-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="5bfc9-103">Update managedMobileApp</span></span>

<span data-ttu-id="5bfc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bfc9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bfc9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bfc9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bfc9-107">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bfc9-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bfc9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5bfc9-108">Prerequisites</span></span>
<span data-ttu-id="5bfc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bfc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bfc9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bfc9-111">Permission type</span></span>|<span data-ttu-id="5bfc9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5bfc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bfc9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bfc9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bfc9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bfc9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bfc9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bfc9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bfc9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-116">Not supported.</span></span>|
|<span data-ttu-id="5bfc9-117">Application</span><span class="sxs-lookup"><span data-stu-id="5bfc9-117">Application</span></span>|<span data-ttu-id="5bfc9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bfc9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bfc9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfc9-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5bfc9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfc9-120">Request headers</span></span>
|<span data-ttu-id="5bfc9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bfc9-121">Header</span></span>|<span data-ttu-id="5bfc9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5bfc9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bfc9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bfc9-123">Authorization</span></span>|<span data-ttu-id="5bfc9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bfc9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5bfc9-125">Accept</span></span>|<span data-ttu-id="5bfc9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5bfc9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bfc9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfc9-127">Request body</span></span>
<span data-ttu-id="5bfc9-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bfc9-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="5bfc9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bfc9-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="5bfc9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bfc9-130">Property</span></span>|<span data-ttu-id="5bfc9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bfc9-131">Type</span></span>|<span data-ttu-id="5bfc9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bfc9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bfc9-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5bfc9-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="5bfc9-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5bfc9-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5bfc9-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="5bfc9-136">id</span><span class="sxs-lookup"><span data-stu-id="5bfc9-136">id</span></span>|<span data-ttu-id="5bfc9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bfc9-137">String</span></span>|<span data-ttu-id="5bfc9-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-138">Key of the entity.</span></span>|
|<span data-ttu-id="5bfc9-139">versão</span><span class="sxs-lookup"><span data-stu-id="5bfc9-139">version</span></span>|<span data-ttu-id="5bfc9-140">String</span><span class="sxs-lookup"><span data-stu-id="5bfc9-140">String</span></span>|<span data-ttu-id="5bfc9-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5bfc9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfc9-142">Response</span></span>
<span data-ttu-id="5bfc9-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bfc9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bfc9-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bfc9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfc9-145">Request</span></span>
<span data-ttu-id="5bfc9-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5bfc9-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfc9-147">Response</span></span>
<span data-ttu-id="5bfc9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bfc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



