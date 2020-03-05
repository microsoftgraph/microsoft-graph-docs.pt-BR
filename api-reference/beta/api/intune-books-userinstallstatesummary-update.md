---
title: Atualizar userInstallStateSummary
description: Atualizar as propriedades de um objeto userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9304647712f9145712b0d6dcf9ba486175e4df4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444473"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="3dc28-103">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="3dc28-103">Update userInstallStateSummary</span></span>

<span data-ttu-id="3dc28-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3dc28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3dc28-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3dc28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dc28-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3dc28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dc28-107">Atualizar as propriedades de um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3dc28-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dc28-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3dc28-108">Prerequisites</span></span>
<span data-ttu-id="3dc28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dc28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dc28-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dc28-111">Permission type</span></span>|<span data-ttu-id="3dc28-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3dc28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dc28-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dc28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3dc28-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc28-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3dc28-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dc28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dc28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dc28-116">Not supported.</span></span>|
|<span data-ttu-id="3dc28-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dc28-117">Application</span></span>|<span data-ttu-id="3dc28-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc28-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dc28-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3dc28-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dc28-120">Request headers</span></span>
|<span data-ttu-id="3dc28-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3dc28-121">Header</span></span>|<span data-ttu-id="3dc28-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3dc28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dc28-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dc28-123">Authorization</span></span>|<span data-ttu-id="3dc28-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dc28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dc28-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3dc28-125">Accept</span></span>|<span data-ttu-id="3dc28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3dc28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dc28-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dc28-127">Request body</span></span>
<span data-ttu-id="3dc28-128">No corpo da solicitação, forneça uma representação JSON do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3dc28-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="3dc28-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3dc28-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="3dc28-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3dc28-130">Property</span></span>|<span data-ttu-id="3dc28-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3dc28-131">Type</span></span>|<span data-ttu-id="3dc28-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dc28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dc28-133">id</span><span class="sxs-lookup"><span data-stu-id="3dc28-133">id</span></span>|<span data-ttu-id="3dc28-134">String</span><span class="sxs-lookup"><span data-stu-id="3dc28-134">String</span></span>|<span data-ttu-id="3dc28-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3dc28-135">Key of the entity.</span></span>|
|<span data-ttu-id="3dc28-136">userName</span><span class="sxs-lookup"><span data-stu-id="3dc28-136">userName</span></span>|<span data-ttu-id="3dc28-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3dc28-137">String</span></span>|<span data-ttu-id="3dc28-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="3dc28-138">User name.</span></span>|
|<span data-ttu-id="3dc28-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3dc28-139">installedDeviceCount</span></span>|<span data-ttu-id="3dc28-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3dc28-140">Int32</span></span>|<span data-ttu-id="3dc28-141">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="3dc28-141">Installed Device Count.</span></span>|
|<span data-ttu-id="3dc28-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3dc28-142">failedDeviceCount</span></span>|<span data-ttu-id="3dc28-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3dc28-143">Int32</span></span>|<span data-ttu-id="3dc28-144">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="3dc28-144">Failed Device Count.</span></span>|
|<span data-ttu-id="3dc28-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3dc28-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="3dc28-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3dc28-146">Int32</span></span>|<span data-ttu-id="3dc28-147">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="3dc28-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3dc28-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dc28-148">Response</span></span>
<span data-ttu-id="3dc28-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dc28-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dc28-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dc28-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dc28-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dc28-151">Request</span></span>
<span data-ttu-id="3dc28-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dc28-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="3dc28-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dc28-153">Response</span></span>
<span data-ttu-id="3dc28-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dc28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





