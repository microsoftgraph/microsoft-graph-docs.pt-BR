---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 58d1c7329a65865080a11b99c6c67724e2e37563
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954462"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="9000c-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="9000c-103">Create managedMobileApp</span></span>

> <span data-ttu-id="9000c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9000c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9000c-105">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9000c-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9000c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9000c-106">Prerequisites</span></span>
<span data-ttu-id="9000c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9000c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9000c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9000c-109">Permission type</span></span>|<span data-ttu-id="9000c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9000c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9000c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9000c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9000c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9000c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9000c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9000c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9000c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9000c-114">Not supported.</span></span>|
|<span data-ttu-id="9000c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9000c-115">Application</span></span>|<span data-ttu-id="9000c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9000c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9000c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9000c-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9000c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9000c-118">Request headers</span></span>
|<span data-ttu-id="9000c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9000c-119">Header</span></span>|<span data-ttu-id="9000c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9000c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9000c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9000c-121">Authorization</span></span>|<span data-ttu-id="9000c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9000c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9000c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9000c-123">Accept</span></span>|<span data-ttu-id="9000c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9000c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9000c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9000c-125">Request body</span></span>
<span data-ttu-id="9000c-126">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="9000c-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="9000c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="9000c-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="9000c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9000c-128">Property</span></span>|<span data-ttu-id="9000c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9000c-129">Type</span></span>|<span data-ttu-id="9000c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9000c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9000c-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9000c-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="9000c-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9000c-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9000c-133">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="9000c-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="9000c-134">id</span><span class="sxs-lookup"><span data-stu-id="9000c-134">id</span></span>|<span data-ttu-id="9000c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9000c-135">String</span></span>|<span data-ttu-id="9000c-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9000c-136">Key of the entity.</span></span>|
|<span data-ttu-id="9000c-137">version</span><span class="sxs-lookup"><span data-stu-id="9000c-137">version</span></span>|<span data-ttu-id="9000c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9000c-138">String</span></span>|<span data-ttu-id="9000c-139">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="9000c-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9000c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9000c-140">Response</span></span>
<span data-ttu-id="9000c-141">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9000c-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9000c-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9000c-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="9000c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9000c-143">Request</span></span>
<span data-ttu-id="9000c-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9000c-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9000c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9000c-145">Response</span></span>
<span data-ttu-id="9000c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9000c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



