---
title: Atualizar managedMobileApp
description: Atualizar as propriedades de um objeto managedMobileApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: daea2d1a64d1e0c50ce5cc3467bf1d87556571d4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363371"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="8a575-103">Atualizar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="8a575-103">Update managedMobileApp</span></span>

> <span data-ttu-id="8a575-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a575-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a575-105">Atualizar as propriedades de um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a575-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a575-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a575-106">Prerequisites</span></span>
<span data-ttu-id="8a575-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a575-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a575-109">Permission type</span></span>|<span data-ttu-id="8a575-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a575-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a575-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a575-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a575-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a575-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a575-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a575-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a575-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a575-114">Not supported.</span></span>|
|<span data-ttu-id="8a575-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a575-115">Application</span></span>|<span data-ttu-id="8a575-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a575-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a575-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a575-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8a575-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a575-118">Request headers</span></span>
|<span data-ttu-id="8a575-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a575-119">Header</span></span>|<span data-ttu-id="8a575-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8a575-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a575-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a575-121">Authorization</span></span>|<span data-ttu-id="8a575-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a575-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a575-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a575-123">Accept</span></span>|<span data-ttu-id="8a575-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8a575-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a575-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a575-125">Request body</span></span>
<span data-ttu-id="8a575-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a575-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="8a575-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a575-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="8a575-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a575-128">Property</span></span>|<span data-ttu-id="8a575-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a575-129">Type</span></span>|<span data-ttu-id="8a575-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a575-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a575-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a575-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="8a575-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a575-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8a575-133">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="8a575-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="8a575-134">id</span><span class="sxs-lookup"><span data-stu-id="8a575-134">id</span></span>|<span data-ttu-id="8a575-135">String</span><span class="sxs-lookup"><span data-stu-id="8a575-135">String</span></span>|<span data-ttu-id="8a575-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a575-136">Key of the entity.</span></span>|
|<span data-ttu-id="8a575-137">versão</span><span class="sxs-lookup"><span data-stu-id="8a575-137">version</span></span>|<span data-ttu-id="8a575-138">String</span><span class="sxs-lookup"><span data-stu-id="8a575-138">String</span></span>|<span data-ttu-id="8a575-139">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a575-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8a575-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a575-140">Response</span></span>
<span data-ttu-id="8a575-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a575-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a575-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a575-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a575-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a575-143">Request</span></span>
<span data-ttu-id="8a575-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a575-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a575-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a575-145">Response</span></span>
<span data-ttu-id="8a575-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a575-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




