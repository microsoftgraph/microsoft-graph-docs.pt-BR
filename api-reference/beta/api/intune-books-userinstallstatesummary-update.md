---
title: Atualizar userInstallStateSummary
description: Atualizar as propriedades de um objeto userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2425dcf85ec210a4934a61e52ac3e02979c45157
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930797"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="8100b-103">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="8100b-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="8100b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8100b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8100b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8100b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8100b-106">Atualizar as propriedades de um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8100b-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8100b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8100b-107">Prerequisites</span></span>
<span data-ttu-id="8100b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8100b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8100b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8100b-110">Permission type</span></span>|<span data-ttu-id="8100b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8100b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8100b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8100b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8100b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8100b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8100b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8100b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8100b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8100b-115">Not supported.</span></span>|
|<span data-ttu-id="8100b-116">Application</span><span class="sxs-lookup"><span data-stu-id="8100b-116">Application</span></span>|<span data-ttu-id="8100b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8100b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8100b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8100b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="8100b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8100b-119">Request headers</span></span>
|<span data-ttu-id="8100b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8100b-120">Header</span></span>|<span data-ttu-id="8100b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8100b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8100b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8100b-122">Authorization</span></span>|<span data-ttu-id="8100b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8100b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8100b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8100b-124">Accept</span></span>|<span data-ttu-id="8100b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8100b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8100b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8100b-126">Request body</span></span>
<span data-ttu-id="8100b-127">No corpo da solicitação, forneça uma representação JSON do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8100b-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="8100b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8100b-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="8100b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8100b-129">Property</span></span>|<span data-ttu-id="8100b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8100b-130">Type</span></span>|<span data-ttu-id="8100b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8100b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8100b-132">id</span><span class="sxs-lookup"><span data-stu-id="8100b-132">id</span></span>|<span data-ttu-id="8100b-133">String</span><span class="sxs-lookup"><span data-stu-id="8100b-133">String</span></span>|<span data-ttu-id="8100b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8100b-134">Key of the entity.</span></span>|
|<span data-ttu-id="8100b-135">userName</span><span class="sxs-lookup"><span data-stu-id="8100b-135">userName</span></span>|<span data-ttu-id="8100b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8100b-136">String</span></span>|<span data-ttu-id="8100b-137">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="8100b-137">User name.</span></span>|
|<span data-ttu-id="8100b-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8100b-138">installedDeviceCount</span></span>|<span data-ttu-id="8100b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8100b-139">Int32</span></span>|<span data-ttu-id="8100b-140">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="8100b-140">Installed Device Count.</span></span>|
|<span data-ttu-id="8100b-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8100b-141">failedDeviceCount</span></span>|<span data-ttu-id="8100b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8100b-142">Int32</span></span>|<span data-ttu-id="8100b-143">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8100b-143">Failed Device Count.</span></span>|
|<span data-ttu-id="8100b-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8100b-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="8100b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8100b-145">Int32</span></span>|<span data-ttu-id="8100b-146">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="8100b-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="8100b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8100b-147">Response</span></span>
<span data-ttu-id="8100b-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8100b-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8100b-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8100b-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8100b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8100b-150">Request</span></span>
<span data-ttu-id="8100b-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8100b-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8100b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8100b-152">Response</span></span>
<span data-ttu-id="8100b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8100b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





