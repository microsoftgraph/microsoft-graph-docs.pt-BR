---
title: Atualizar userInstallStateSummary
description: Atualizar as propriedades de um objeto userInstallStateSummary.
ms.openlocfilehash: a5c3f1278a8c9696b65663eaaeafcb76e1e09840
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003556"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="a039f-103">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="a039f-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="a039f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a039f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a039f-105">Atualizar as propriedades de um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a039f-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a039f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a039f-106">Prerequisites</span></span>
<span data-ttu-id="a039f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a039f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a039f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a039f-109">Permission type</span></span>|<span data-ttu-id="a039f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a039f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a039f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a039f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a039f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a039f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a039f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a039f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a039f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a039f-114">Not supported.</span></span>|
|<span data-ttu-id="a039f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a039f-115">Application</span></span>|<span data-ttu-id="a039f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a039f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a039f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a039f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a039f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a039f-118">Request headers</span></span>
|<span data-ttu-id="a039f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a039f-119">Header</span></span>|<span data-ttu-id="a039f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a039f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a039f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a039f-121">Authorization</span></span>|<span data-ttu-id="a039f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a039f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a039f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a039f-123">Accept</span></span>|<span data-ttu-id="a039f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a039f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a039f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a039f-125">Request body</span></span>
<span data-ttu-id="a039f-126">No corpo da solicitação, forneça uma representação JSON do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a039f-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="a039f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a039f-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="a039f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a039f-128">Property</span></span>|<span data-ttu-id="a039f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a039f-129">Type</span></span>|<span data-ttu-id="a039f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a039f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a039f-131">id</span><span class="sxs-lookup"><span data-stu-id="a039f-131">id</span></span>|<span data-ttu-id="a039f-132">String</span><span class="sxs-lookup"><span data-stu-id="a039f-132">String</span></span>|<span data-ttu-id="a039f-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a039f-133">Key of the entity.</span></span>|
|<span data-ttu-id="a039f-134">userName</span><span class="sxs-lookup"><span data-stu-id="a039f-134">userName</span></span>|<span data-ttu-id="a039f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a039f-135">String</span></span>|<span data-ttu-id="a039f-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="a039f-136">User name.</span></span>|
|<span data-ttu-id="a039f-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a039f-137">installedDeviceCount</span></span>|<span data-ttu-id="a039f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a039f-138">Int32</span></span>|<span data-ttu-id="a039f-139">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="a039f-139">Installed Device Count.</span></span>|
|<span data-ttu-id="a039f-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a039f-140">failedDeviceCount</span></span>|<span data-ttu-id="a039f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a039f-141">Int32</span></span>|<span data-ttu-id="a039f-142">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a039f-142">Failed Device Count.</span></span>|
|<span data-ttu-id="a039f-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a039f-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="a039f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a039f-144">Int32</span></span>|<span data-ttu-id="a039f-145">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="a039f-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="a039f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a039f-146">Response</span></span>
<span data-ttu-id="a039f-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a039f-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a039f-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a039f-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a039f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a039f-149">Request</span></span>
<span data-ttu-id="a039f-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a039f-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="a039f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a039f-151">Response</span></span>
<span data-ttu-id="a039f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a039f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



