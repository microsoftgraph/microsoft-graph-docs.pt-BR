---
title: Atualizar eBookInstallSummary
description: Atualizar as propriedades de um objeto eBookInstallSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56f16314672e5b5beb8a3a7fbeee5693aca4e4ca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126924"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="df949-103">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="df949-103">Update eBookInstallSummary</span></span>

<span data-ttu-id="df949-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df949-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df949-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df949-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df949-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df949-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df949-107">Atualizar as propriedades de um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="df949-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df949-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df949-108">Prerequisites</span></span>
<span data-ttu-id="df949-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df949-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df949-111">Permission type</span></span>|<span data-ttu-id="df949-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df949-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df949-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df949-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df949-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df949-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df949-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df949-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df949-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df949-116">Not supported.</span></span>|
|<span data-ttu-id="df949-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df949-117">Application</span></span>|<span data-ttu-id="df949-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df949-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df949-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df949-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="df949-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df949-120">Request headers</span></span>
|<span data-ttu-id="df949-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df949-121">Header</span></span>|<span data-ttu-id="df949-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df949-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df949-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df949-123">Authorization</span></span>|<span data-ttu-id="df949-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df949-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df949-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df949-125">Accept</span></span>|<span data-ttu-id="df949-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df949-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df949-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df949-127">Request body</span></span>
<span data-ttu-id="df949-128">No corpo da solicitação, forneça uma representação JSON do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="df949-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="df949-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="df949-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="df949-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df949-130">Property</span></span>|<span data-ttu-id="df949-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df949-131">Type</span></span>|<span data-ttu-id="df949-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df949-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df949-133">id</span><span class="sxs-lookup"><span data-stu-id="df949-133">id</span></span>|<span data-ttu-id="df949-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df949-134">String</span></span>|<span data-ttu-id="df949-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df949-135">Key of the entity.</span></span>|
|<span data-ttu-id="df949-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df949-136">installedDeviceCount</span></span>|<span data-ttu-id="df949-137">Int32</span><span class="sxs-lookup"><span data-stu-id="df949-137">Int32</span></span>|<span data-ttu-id="df949-138">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="df949-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="df949-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df949-139">failedDeviceCount</span></span>|<span data-ttu-id="df949-140">Int32</span><span class="sxs-lookup"><span data-stu-id="df949-140">Int32</span></span>|<span data-ttu-id="df949-141">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="df949-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="df949-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df949-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="df949-143">Int32</span><span class="sxs-lookup"><span data-stu-id="df949-143">Int32</span></span>|<span data-ttu-id="df949-144">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="df949-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="df949-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="df949-145">installedUserCount</span></span>|<span data-ttu-id="df949-146">Int32</span><span class="sxs-lookup"><span data-stu-id="df949-146">Int32</span></span>|<span data-ttu-id="df949-147">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="df949-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="df949-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="df949-148">failedUserCount</span></span>|<span data-ttu-id="df949-149">Int32</span><span class="sxs-lookup"><span data-stu-id="df949-149">Int32</span></span>|<span data-ttu-id="df949-150">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="df949-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="df949-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="df949-151">notInstalledUserCount</span></span>|<span data-ttu-id="df949-152">Int32</span><span class="sxs-lookup"><span data-stu-id="df949-152">Int32</span></span>|<span data-ttu-id="df949-153">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="df949-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="df949-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="df949-154">Response</span></span>
<span data-ttu-id="df949-155">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df949-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df949-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df949-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="df949-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df949-157">Request</span></span>
<span data-ttu-id="df949-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df949-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
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

### <a name="response"></a><span data-ttu-id="df949-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="df949-159">Response</span></span>
<span data-ttu-id="df949-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df949-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




