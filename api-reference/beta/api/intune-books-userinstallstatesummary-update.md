---
title: Atualizar userInstallStateSummary
description: Atualizar as propriedades de um objeto userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96f292579ced40b378e2f4af01ef50a0309daea6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690165"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="07b34-103">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="07b34-103">Update userInstallStateSummary</span></span>

<span data-ttu-id="07b34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07b34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07b34-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07b34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07b34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07b34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07b34-107">Atualizar as propriedades de um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="07b34-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07b34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07b34-108">Prerequisites</span></span>
<span data-ttu-id="07b34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07b34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07b34-111">Permission type</span></span>|<span data-ttu-id="07b34-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07b34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07b34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07b34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07b34-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b34-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07b34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07b34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07b34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07b34-116">Not supported.</span></span>|
|<span data-ttu-id="07b34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07b34-117">Application</span></span>|<span data-ttu-id="07b34-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b34-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07b34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07b34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="07b34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07b34-120">Request headers</span></span>
|<span data-ttu-id="07b34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07b34-121">Header</span></span>|<span data-ttu-id="07b34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07b34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07b34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07b34-123">Authorization</span></span>|<span data-ttu-id="07b34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07b34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07b34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07b34-125">Accept</span></span>|<span data-ttu-id="07b34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07b34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07b34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07b34-127">Request body</span></span>
<span data-ttu-id="07b34-128">No corpo da solicitação, forneça uma representação JSON do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="07b34-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="07b34-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="07b34-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="07b34-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07b34-130">Property</span></span>|<span data-ttu-id="07b34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07b34-131">Type</span></span>|<span data-ttu-id="07b34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07b34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07b34-133">id</span><span class="sxs-lookup"><span data-stu-id="07b34-133">id</span></span>|<span data-ttu-id="07b34-134">String</span><span class="sxs-lookup"><span data-stu-id="07b34-134">String</span></span>|<span data-ttu-id="07b34-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07b34-135">Key of the entity.</span></span>|
|<span data-ttu-id="07b34-136">userName</span><span class="sxs-lookup"><span data-stu-id="07b34-136">userName</span></span>|<span data-ttu-id="07b34-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07b34-137">String</span></span>|<span data-ttu-id="07b34-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="07b34-138">User name.</span></span>|
|<span data-ttu-id="07b34-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07b34-139">installedDeviceCount</span></span>|<span data-ttu-id="07b34-140">Int32</span><span class="sxs-lookup"><span data-stu-id="07b34-140">Int32</span></span>|<span data-ttu-id="07b34-141">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="07b34-141">Installed Device Count.</span></span>|
|<span data-ttu-id="07b34-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07b34-142">failedDeviceCount</span></span>|<span data-ttu-id="07b34-143">Int32</span><span class="sxs-lookup"><span data-stu-id="07b34-143">Int32</span></span>|<span data-ttu-id="07b34-144">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="07b34-144">Failed Device Count.</span></span>|
|<span data-ttu-id="07b34-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07b34-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="07b34-146">Int32</span><span class="sxs-lookup"><span data-stu-id="07b34-146">Int32</span></span>|<span data-ttu-id="07b34-147">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="07b34-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="07b34-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b34-148">Response</span></span>
<span data-ttu-id="07b34-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07b34-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07b34-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07b34-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="07b34-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07b34-151">Request</span></span>
<span data-ttu-id="07b34-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07b34-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07b34-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b34-153">Response</span></span>
<span data-ttu-id="07b34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07b34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





