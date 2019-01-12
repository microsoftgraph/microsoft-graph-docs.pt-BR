---
title: Criar userInstallStateSummary
description: Criar um novo objeto userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 32f7b427143c8fa1d31302d51417c330cd3ca32d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985904"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="3c9f1-103">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="3c9f1-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="3c9f1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c9f1-105">Criar um novo objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3c9f1-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c9f1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c9f1-106">Prerequisites</span></span>
<span data-ttu-id="3c9f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c9f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c9f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c9f1-109">Permission type</span></span>|<span data-ttu-id="3c9f1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c9f1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c9f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c9f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c9f1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c9f1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c9f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c9f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c9f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-114">Not supported.</span></span>|
|<span data-ttu-id="3c9f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c9f1-115">Application</span></span>|<span data-ttu-id="3c9f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c9f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c9f1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3c9f1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c9f1-118">Request headers</span></span>
|<span data-ttu-id="3c9f1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c9f1-119">Header</span></span>|<span data-ttu-id="3c9f1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3c9f1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c9f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c9f1-121">Authorization</span></span>|<span data-ttu-id="3c9f1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c9f1-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c9f1-123">Accept</span></span>|<span data-ttu-id="3c9f1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c9f1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c9f1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c9f1-125">Request body</span></span>
<span data-ttu-id="3c9f1-126">No corpo da solicitação, forneça uma representação JSON do objeto userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="3c9f1-127">A tabela a seguir mostra as propriedades que são necessárias ao criar userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="3c9f1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c9f1-128">Property</span></span>|<span data-ttu-id="3c9f1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c9f1-129">Type</span></span>|<span data-ttu-id="3c9f1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c9f1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c9f1-131">id</span><span class="sxs-lookup"><span data-stu-id="3c9f1-131">id</span></span>|<span data-ttu-id="3c9f1-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c9f1-132">String</span></span>|<span data-ttu-id="3c9f1-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-133">Key of the entity.</span></span>|
|<span data-ttu-id="3c9f1-134">userName</span><span class="sxs-lookup"><span data-stu-id="3c9f1-134">userName</span></span>|<span data-ttu-id="3c9f1-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c9f1-135">String</span></span>|<span data-ttu-id="3c9f1-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-136">User name.</span></span>|
|<span data-ttu-id="3c9f1-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c9f1-137">installedDeviceCount</span></span>|<span data-ttu-id="3c9f1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3c9f1-138">Int32</span></span>|<span data-ttu-id="3c9f1-139">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-139">Installed Device Count.</span></span>|
|<span data-ttu-id="3c9f1-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c9f1-140">failedDeviceCount</span></span>|<span data-ttu-id="3c9f1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3c9f1-141">Int32</span></span>|<span data-ttu-id="3c9f1-142">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-142">Failed Device Count.</span></span>|
|<span data-ttu-id="3c9f1-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c9f1-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="3c9f1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3c9f1-144">Int32</span></span>|<span data-ttu-id="3c9f1-145">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3c9f1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c9f1-146">Response</span></span>
<span data-ttu-id="3c9f1-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c9f1-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c9f1-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c9f1-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c9f1-149">Request</span></span>
<span data-ttu-id="3c9f1-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="3c9f1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c9f1-151">Response</span></span>
<span data-ttu-id="3c9f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c9f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```



