---
title: Criar userInstallStateSummary
description: Criar um novo objeto userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cb123adec686db29bdf1dfefc3c7a459a427833
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989369"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="9d16a-103">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="9d16a-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="9d16a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d16a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d16a-105">Criar um novo objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9d16a-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d16a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d16a-106">Prerequisites</span></span>
<span data-ttu-id="9d16a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d16a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d16a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d16a-109">Permission type</span></span>|<span data-ttu-id="9d16a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d16a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d16a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d16a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d16a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d16a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d16a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d16a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d16a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d16a-114">Not supported.</span></span>|
|<span data-ttu-id="9d16a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d16a-115">Application</span></span>|<span data-ttu-id="9d16a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d16a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d16a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d16a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="9d16a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d16a-118">Request headers</span></span>
|<span data-ttu-id="9d16a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d16a-119">Header</span></span>|<span data-ttu-id="9d16a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9d16a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d16a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d16a-121">Authorization</span></span>|<span data-ttu-id="9d16a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d16a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d16a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d16a-123">Accept</span></span>|<span data-ttu-id="9d16a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d16a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d16a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d16a-125">Request body</span></span>
<span data-ttu-id="9d16a-126">No corpo da solicitação, forneça uma representação JSON do objeto userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="9d16a-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="9d16a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="9d16a-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="9d16a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d16a-128">Property</span></span>|<span data-ttu-id="9d16a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d16a-129">Type</span></span>|<span data-ttu-id="9d16a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d16a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d16a-131">id</span><span class="sxs-lookup"><span data-stu-id="9d16a-131">id</span></span>|<span data-ttu-id="9d16a-132">String</span><span class="sxs-lookup"><span data-stu-id="9d16a-132">String</span></span>|<span data-ttu-id="9d16a-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d16a-133">Key of the entity.</span></span>|
|<span data-ttu-id="9d16a-134">userName</span><span class="sxs-lookup"><span data-stu-id="9d16a-134">userName</span></span>|<span data-ttu-id="9d16a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d16a-135">String</span></span>|<span data-ttu-id="9d16a-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="9d16a-136">User name.</span></span>|
|<span data-ttu-id="9d16a-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d16a-137">installedDeviceCount</span></span>|<span data-ttu-id="9d16a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9d16a-138">Int32</span></span>|<span data-ttu-id="9d16a-139">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="9d16a-139">Installed Device Count.</span></span>|
|<span data-ttu-id="9d16a-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d16a-140">failedDeviceCount</span></span>|<span data-ttu-id="9d16a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9d16a-141">Int32</span></span>|<span data-ttu-id="9d16a-142">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9d16a-142">Failed Device Count.</span></span>|
|<span data-ttu-id="9d16a-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d16a-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="9d16a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9d16a-144">Int32</span></span>|<span data-ttu-id="9d16a-145">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="9d16a-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="9d16a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d16a-146">Response</span></span>
<span data-ttu-id="9d16a-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d16a-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d16a-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d16a-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d16a-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d16a-149">Request</span></span>
<span data-ttu-id="9d16a-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d16a-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d16a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d16a-151">Response</span></span>
<span data-ttu-id="9d16a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d16a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



