---
title: Atualizar eBookInstallSummary
description: Atualizar as propriedades de um objeto eBookInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3053911b32e0850009adb42815114adc6c2848b2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758705"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="c335c-103">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c335c-103">Update eBookInstallSummary</span></span>

<span data-ttu-id="c335c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c335c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c335c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c335c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c335c-106">Atualizar as propriedades de um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c335c-106">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c335c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c335c-107">Prerequisites</span></span>
<span data-ttu-id="c335c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c335c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c335c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c335c-110">Permission type</span></span>|<span data-ttu-id="c335c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c335c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c335c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c335c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c335c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c335c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c335c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c335c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c335c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c335c-115">Not supported.</span></span>|
|<span data-ttu-id="c335c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c335c-116">Application</span></span>|<span data-ttu-id="c335c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c335c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c335c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c335c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="c335c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c335c-119">Request headers</span></span>
|<span data-ttu-id="c335c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c335c-120">Header</span></span>|<span data-ttu-id="c335c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c335c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c335c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c335c-122">Authorization</span></span>|<span data-ttu-id="c335c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c335c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c335c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c335c-124">Accept</span></span>|<span data-ttu-id="c335c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c335c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c335c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c335c-126">Request body</span></span>
<span data-ttu-id="c335c-127">No corpo da solicitação, forneça uma representação JSON do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c335c-127">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="c335c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c335c-128">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="c335c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c335c-129">Property</span></span>|<span data-ttu-id="c335c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c335c-130">Type</span></span>|<span data-ttu-id="c335c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c335c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c335c-132">id</span><span class="sxs-lookup"><span data-stu-id="c335c-132">id</span></span>|<span data-ttu-id="c335c-133">String</span><span class="sxs-lookup"><span data-stu-id="c335c-133">String</span></span>|<span data-ttu-id="c335c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c335c-134">Key of the entity.</span></span>|
|<span data-ttu-id="c335c-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c335c-135">installedDeviceCount</span></span>|<span data-ttu-id="c335c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c335c-136">Int32</span></span>|<span data-ttu-id="c335c-137">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="c335c-137">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="c335c-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c335c-138">failedDeviceCount</span></span>|<span data-ttu-id="c335c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c335c-139">Int32</span></span>|<span data-ttu-id="c335c-140">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="c335c-140">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="c335c-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c335c-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="c335c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c335c-142">Int32</span></span>|<span data-ttu-id="c335c-143">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="c335c-143">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="c335c-144">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="c335c-144">installedUserCount</span></span>|<span data-ttu-id="c335c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c335c-145">Int32</span></span>|<span data-ttu-id="c335c-146">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="c335c-146">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="c335c-147">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="c335c-147">failedUserCount</span></span>|<span data-ttu-id="c335c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c335c-148">Int32</span></span>|<span data-ttu-id="c335c-149">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="c335c-149">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="c335c-150">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="c335c-150">notInstalledUserCount</span></span>|<span data-ttu-id="c335c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c335c-151">Int32</span></span>|<span data-ttu-id="c335c-152">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="c335c-152">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="c335c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c335c-153">Response</span></span>
<span data-ttu-id="c335c-154">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c335c-154">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c335c-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c335c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c335c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c335c-156">Request</span></span>
<span data-ttu-id="c335c-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c335c-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="c335c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c335c-158">Response</span></span>
<span data-ttu-id="c335c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c335c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```




