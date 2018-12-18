---
title: Atualizar eBookInstallSummary
description: Atualizar as propriedades de um objeto eBookInstallSummary.
author: tfitzmac
ms.openlocfilehash: b110646f51ce8c48e15bd8c5fbaa5e025952babc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350726"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="ce587-103">Atualizar eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ce587-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="ce587-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce587-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce587-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce587-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce587-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ce587-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce587-107">Atualizar as propriedades de um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ce587-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce587-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce587-108">Prerequisites</span></span>
<span data-ttu-id="ce587-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce587-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce587-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce587-111">Permission type</span></span>|<span data-ttu-id="ce587-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce587-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce587-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce587-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce587-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce587-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce587-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce587-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce587-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce587-116">Not supported.</span></span>|
|<span data-ttu-id="ce587-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce587-117">Application</span></span>|<span data-ttu-id="ce587-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce587-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce587-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce587-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="ce587-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce587-120">Request headers</span></span>
|<span data-ttu-id="ce587-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce587-121">Header</span></span>|<span data-ttu-id="ce587-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ce587-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce587-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce587-123">Authorization</span></span>|<span data-ttu-id="ce587-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce587-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce587-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce587-125">Accept</span></span>|<span data-ttu-id="ce587-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce587-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce587-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce587-127">Request body</span></span>
<span data-ttu-id="ce587-128">No corpo da solicitação, forneça uma representação JSON do objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ce587-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="ce587-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ce587-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="ce587-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce587-130">Property</span></span>|<span data-ttu-id="ce587-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce587-131">Type</span></span>|<span data-ttu-id="ce587-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce587-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce587-133">id</span><span class="sxs-lookup"><span data-stu-id="ce587-133">id</span></span>|<span data-ttu-id="ce587-134">String</span><span class="sxs-lookup"><span data-stu-id="ce587-134">String</span></span>|<span data-ttu-id="ce587-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce587-135">Key of the entity.</span></span>|
|<span data-ttu-id="ce587-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce587-136">installedDeviceCount</span></span>|<span data-ttu-id="ce587-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ce587-137">Int32</span></span>|<span data-ttu-id="ce587-138">Número de dispositivos que instalaram este livro com êxito.</span><span class="sxs-lookup"><span data-stu-id="ce587-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ce587-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce587-139">failedDeviceCount</span></span>|<span data-ttu-id="ce587-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ce587-140">Int32</span></span>|<span data-ttu-id="ce587-141">Número de dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="ce587-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ce587-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ce587-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="ce587-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ce587-143">Int32</span></span>|<span data-ttu-id="ce587-144">Número de dispositivos que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="ce587-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ce587-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ce587-145">installedUserCount</span></span>|<span data-ttu-id="ce587-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ce587-146">Int32</span></span>|<span data-ttu-id="ce587-147">Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="ce587-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ce587-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ce587-148">failedUserCount</span></span>|<span data-ttu-id="ce587-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ce587-149">Int32</span></span>|<span data-ttu-id="ce587-150">Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.</span><span class="sxs-lookup"><span data-stu-id="ce587-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ce587-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ce587-151">notInstalledUserCount</span></span>|<span data-ttu-id="ce587-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ce587-152">Int32</span></span>|<span data-ttu-id="ce587-153">Número de usuários que não instalaram este livro.</span><span class="sxs-lookup"><span data-stu-id="ce587-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="ce587-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce587-154">Response</span></span>
<span data-ttu-id="ce587-155">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce587-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce587-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce587-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce587-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce587-157">Request</span></span>
<span data-ttu-id="ce587-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce587-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="ce587-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce587-159">Response</span></span>
<span data-ttu-id="ce587-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce587-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





