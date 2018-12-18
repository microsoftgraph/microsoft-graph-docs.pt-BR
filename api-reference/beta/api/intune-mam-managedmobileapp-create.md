---
title: Criar managedMobileApp
description: Criar um novo objeto managedMobileApp.
author: tfitzmac
ms.openlocfilehash: 07db13e6f38039c153eed44f401f3e2d846840ee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321193"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="7538b-103">Criar managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="7538b-103">Create managedMobileApp</span></span>

> <span data-ttu-id="7538b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7538b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7538b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7538b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7538b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7538b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7538b-107">Criar um novo objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7538b-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7538b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7538b-108">Prerequisites</span></span>
<span data-ttu-id="7538b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7538b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7538b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7538b-111">Permission type</span></span>|<span data-ttu-id="7538b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7538b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7538b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7538b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7538b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7538b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7538b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7538b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7538b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7538b-116">Not supported.</span></span>|
|<span data-ttu-id="7538b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7538b-117">Application</span></span>|<span data-ttu-id="7538b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7538b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7538b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7538b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7538b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7538b-120">Request headers</span></span>
|<span data-ttu-id="7538b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7538b-121">Header</span></span>|<span data-ttu-id="7538b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7538b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7538b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7538b-123">Authorization</span></span>|<span data-ttu-id="7538b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7538b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7538b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7538b-125">Accept</span></span>|<span data-ttu-id="7538b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7538b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7538b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7538b-127">Request body</span></span>
<span data-ttu-id="7538b-128">No corpo da solicitação, forneça uma representação JSON do objeto managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="7538b-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="7538b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="7538b-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="7538b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7538b-130">Property</span></span>|<span data-ttu-id="7538b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7538b-131">Type</span></span>|<span data-ttu-id="7538b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7538b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7538b-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7538b-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="7538b-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7538b-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="7538b-135">O identificador de um aplicativo com seu tipo de sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="7538b-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="7538b-136">id</span><span class="sxs-lookup"><span data-stu-id="7538b-136">id</span></span>|<span data-ttu-id="7538b-137">String</span><span class="sxs-lookup"><span data-stu-id="7538b-137">String</span></span>|<span data-ttu-id="7538b-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7538b-138">Key of the entity.</span></span>|
|<span data-ttu-id="7538b-139">version</span><span class="sxs-lookup"><span data-stu-id="7538b-139">version</span></span>|<span data-ttu-id="7538b-140">String</span><span class="sxs-lookup"><span data-stu-id="7538b-140">String</span></span>|<span data-ttu-id="7538b-141">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7538b-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="7538b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7538b-142">Response</span></span>
<span data-ttu-id="7538b-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [managedMobileApp](../resources/intune-mam-managedmobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7538b-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7538b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7538b-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="7538b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7538b-145">Request</span></span>
<span data-ttu-id="7538b-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7538b-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="7538b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7538b-147">Response</span></span>
<span data-ttu-id="7538b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7538b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





