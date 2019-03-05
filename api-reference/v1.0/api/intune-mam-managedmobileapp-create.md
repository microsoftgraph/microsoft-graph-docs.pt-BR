---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5eef2246ab45c82a0b4359c00e0e8ec61e3f89c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256613"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="7aaa1-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="7aaa1-103">Create managedMobileApp</span></span>

> <span data-ttu-id="7aaa1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aaa1-105">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7aaa1-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7aaa1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7aaa1-106">Prerequisites</span></span>
<span data-ttu-id="7aaa1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7aaa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7aaa1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aaa1-109">Permission type</span></span>|<span data-ttu-id="7aaa1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7aaa1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aaa1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aaa1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7aaa1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aaa1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7aaa1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aaa1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aaa1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-114">Not supported.</span></span>|
|<span data-ttu-id="7aaa1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aaa1-115">Application</span></span>|<span data-ttu-id="7aaa1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aaa1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aaa1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="7aaa1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aaa1-118">Request headers</span></span>
|<span data-ttu-id="7aaa1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7aaa1-119">Header</span></span>|<span data-ttu-id="7aaa1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7aaa1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aaa1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aaa1-121">Authorization</span></span>|<span data-ttu-id="7aaa1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aaa1-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7aaa1-123">Accept</span></span>|<span data-ttu-id="7aaa1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7aaa1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aaa1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aaa1-125">Request body</span></span>
<span data-ttu-id="7aaa1-126">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="7aaa1-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="7aaa1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aaa1-128">Property</span></span>|<span data-ttu-id="7aaa1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aaa1-129">Type</span></span>|<span data-ttu-id="7aaa1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aaa1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aaa1-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7aaa1-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="7aaa1-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7aaa1-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="7aaa1-133">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="7aaa1-134">id</span><span class="sxs-lookup"><span data-stu-id="7aaa1-134">id</span></span>|<span data-ttu-id="7aaa1-135">String</span><span class="sxs-lookup"><span data-stu-id="7aaa1-135">String</span></span>|<span data-ttu-id="7aaa1-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-136">Key of the entity.</span></span>|
|<span data-ttu-id="7aaa1-137">version</span><span class="sxs-lookup"><span data-stu-id="7aaa1-137">version</span></span>|<span data-ttu-id="7aaa1-138">String</span><span class="sxs-lookup"><span data-stu-id="7aaa1-138">String</span></span>|<span data-ttu-id="7aaa1-139">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="7aaa1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aaa1-140">Response</span></span>
<span data-ttu-id="7aaa1-141">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aaa1-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7aaa1-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="7aaa1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aaa1-143">Request</span></span>
<span data-ttu-id="7aaa1-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="7aaa1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aaa1-145">Response</span></span>
<span data-ttu-id="7aaa1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aaa1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



