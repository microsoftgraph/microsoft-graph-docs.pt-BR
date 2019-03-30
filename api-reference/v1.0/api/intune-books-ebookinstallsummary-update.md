---
title: Atualizar eBookInstallSummary
description: Atualizar as propriedades de um objeto eBookInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f9927dc4c757a83afa02f101815536b1b81d81e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988851"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="2fa85-103">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2fa85-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="2fa85-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fa85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fa85-105">Atualizar as propriedades de um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2fa85-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fa85-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fa85-106">Prerequisites</span></span>
<span data-ttu-id="2fa85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fa85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fa85-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fa85-109">Permission type</span></span>|<span data-ttu-id="2fa85-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2fa85-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fa85-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fa85-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2fa85-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fa85-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2fa85-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fa85-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fa85-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fa85-114">Not supported.</span></span>|
|<span data-ttu-id="2fa85-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fa85-115">Application</span></span>|<span data-ttu-id="2fa85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fa85-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fa85-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fa85-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="2fa85-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa85-118">Request headers</span></span>
|<span data-ttu-id="2fa85-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fa85-119">Header</span></span>|<span data-ttu-id="2fa85-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2fa85-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fa85-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fa85-121">Authorization</span></span>|<span data-ttu-id="2fa85-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fa85-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fa85-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2fa85-123">Accept</span></span>|<span data-ttu-id="2fa85-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2fa85-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fa85-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa85-125">Request body</span></span>
<span data-ttu-id="2fa85-126">No corpo da solicitação, forneça uma representação JSON do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2fa85-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="2fa85-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2fa85-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="2fa85-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fa85-128">Property</span></span>|<span data-ttu-id="2fa85-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa85-129">Type</span></span>|<span data-ttu-id="2fa85-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fa85-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa85-131">id</span><span class="sxs-lookup"><span data-stu-id="2fa85-131">id</span></span>|<span data-ttu-id="2fa85-132">String</span><span class="sxs-lookup"><span data-stu-id="2fa85-132">String</span></span>|<span data-ttu-id="2fa85-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2fa85-133">Key of the entity.</span></span>|
|<span data-ttu-id="2fa85-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2fa85-134">installedDeviceCount</span></span>|<span data-ttu-id="2fa85-135">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa85-135">Int32</span></span>|<span data-ttu-id="2fa85-136">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="2fa85-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="2fa85-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2fa85-137">failedDeviceCount</span></span>|<span data-ttu-id="2fa85-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa85-138">Int32</span></span>|<span data-ttu-id="2fa85-139">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="2fa85-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="2fa85-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2fa85-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="2fa85-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa85-141">Int32</span></span>|<span data-ttu-id="2fa85-142">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="2fa85-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="2fa85-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="2fa85-143">installedUserCount</span></span>|<span data-ttu-id="2fa85-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa85-144">Int32</span></span>|<span data-ttu-id="2fa85-145">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="2fa85-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="2fa85-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="2fa85-146">failedUserCount</span></span>|<span data-ttu-id="2fa85-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa85-147">Int32</span></span>|<span data-ttu-id="2fa85-148">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="2fa85-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="2fa85-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="2fa85-149">notInstalledUserCount</span></span>|<span data-ttu-id="2fa85-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2fa85-150">Int32</span></span>|<span data-ttu-id="2fa85-151">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="2fa85-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="2fa85-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fa85-152">Response</span></span>
<span data-ttu-id="2fa85-153">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fa85-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fa85-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fa85-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fa85-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa85-155">Request</span></span>
<span data-ttu-id="2fa85-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fa85-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2fa85-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fa85-157">Response</span></span>
<span data-ttu-id="2fa85-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fa85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



