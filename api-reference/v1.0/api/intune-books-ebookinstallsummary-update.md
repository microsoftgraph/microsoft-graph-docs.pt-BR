---
title: Atualizar eBookInstallSummary
description: Atualizar as propriedades de um objeto eBookInstallSummary.
ms.openlocfilehash: 261dd70883992b2aa1b2d480407969c1c887c421
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003719"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="a387c-103">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a387c-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="a387c-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a387c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a387c-105">Atualizar as propriedades de um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a387c-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a387c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a387c-106">Prerequisites</span></span>
<span data-ttu-id="a387c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a387c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a387c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a387c-109">Permission type</span></span>|<span data-ttu-id="a387c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a387c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a387c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a387c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a387c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a387c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a387c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a387c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a387c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a387c-114">Not supported.</span></span>|
|<span data-ttu-id="a387c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a387c-115">Application</span></span>|<span data-ttu-id="a387c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a387c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a387c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a387c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="a387c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a387c-118">Request headers</span></span>
|<span data-ttu-id="a387c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a387c-119">Header</span></span>|<span data-ttu-id="a387c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a387c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a387c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a387c-121">Authorization</span></span>|<span data-ttu-id="a387c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a387c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a387c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a387c-123">Accept</span></span>|<span data-ttu-id="a387c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a387c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a387c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a387c-125">Request body</span></span>
<span data-ttu-id="a387c-126">No corpo da solicitação, forneça uma representação JSON do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a387c-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="a387c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a387c-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="a387c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a387c-128">Property</span></span>|<span data-ttu-id="a387c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a387c-129">Type</span></span>|<span data-ttu-id="a387c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a387c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a387c-131">id</span><span class="sxs-lookup"><span data-stu-id="a387c-131">id</span></span>|<span data-ttu-id="a387c-132">String</span><span class="sxs-lookup"><span data-stu-id="a387c-132">String</span></span>|<span data-ttu-id="a387c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a387c-133">Key of the entity.</span></span>|
|<span data-ttu-id="a387c-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a387c-134">installedDeviceCount</span></span>|<span data-ttu-id="a387c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a387c-135">Int32</span></span>|<span data-ttu-id="a387c-136">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="a387c-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="a387c-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a387c-137">failedDeviceCount</span></span>|<span data-ttu-id="a387c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a387c-138">Int32</span></span>|<span data-ttu-id="a387c-139">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="a387c-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="a387c-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a387c-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="a387c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a387c-141">Int32</span></span>|<span data-ttu-id="a387c-142">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="a387c-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="a387c-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="a387c-143">installedUserCount</span></span>|<span data-ttu-id="a387c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a387c-144">Int32</span></span>|<span data-ttu-id="a387c-145">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="a387c-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="a387c-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="a387c-146">failedUserCount</span></span>|<span data-ttu-id="a387c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a387c-147">Int32</span></span>|<span data-ttu-id="a387c-148">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="a387c-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="a387c-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="a387c-149">notInstalledUserCount</span></span>|<span data-ttu-id="a387c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a387c-150">Int32</span></span>|<span data-ttu-id="a387c-151">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="a387c-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="a387c-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a387c-152">Response</span></span>
<span data-ttu-id="a387c-153">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a387c-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a387c-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a387c-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="a387c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a387c-155">Request</span></span>
<span data-ttu-id="a387c-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a387c-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a387c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a387c-157">Response</span></span>
<span data-ttu-id="a387c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a387c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



