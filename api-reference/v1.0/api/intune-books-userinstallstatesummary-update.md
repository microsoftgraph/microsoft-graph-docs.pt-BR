---
title: Atualizar userInstallStateSummary
description: Atualizar as propriedades de um objeto userInstallStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f3c923a4683227a454c5bf4fae620f44733086c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354620"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="e3eac-103">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="e3eac-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="e3eac-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3eac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3eac-105">Atualizar as propriedades de um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3eac-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3eac-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3eac-106">Prerequisites</span></span>
<span data-ttu-id="e3eac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3eac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3eac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3eac-109">Permission type</span></span>|<span data-ttu-id="e3eac-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3eac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3eac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3eac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3eac-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3eac-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3eac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3eac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3eac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3eac-114">Not supported.</span></span>|
|<span data-ttu-id="e3eac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3eac-115">Application</span></span>|<span data-ttu-id="e3eac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3eac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3eac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3eac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e3eac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3eac-118">Request headers</span></span>
|<span data-ttu-id="e3eac-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3eac-119">Header</span></span>|<span data-ttu-id="e3eac-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e3eac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3eac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3eac-121">Authorization</span></span>|<span data-ttu-id="e3eac-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3eac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3eac-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3eac-123">Accept</span></span>|<span data-ttu-id="e3eac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3eac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3eac-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3eac-125">Request body</span></span>
<span data-ttu-id="e3eac-126">No corpo da solicitação, forneça uma representação JSON do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3eac-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="e3eac-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e3eac-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="e3eac-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3eac-128">Property</span></span>|<span data-ttu-id="e3eac-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3eac-129">Type</span></span>|<span data-ttu-id="e3eac-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3eac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3eac-131">id</span><span class="sxs-lookup"><span data-stu-id="e3eac-131">id</span></span>|<span data-ttu-id="e3eac-132">String</span><span class="sxs-lookup"><span data-stu-id="e3eac-132">String</span></span>|<span data-ttu-id="e3eac-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e3eac-133">Key of the entity.</span></span>|
|<span data-ttu-id="e3eac-134">userName</span><span class="sxs-lookup"><span data-stu-id="e3eac-134">userName</span></span>|<span data-ttu-id="e3eac-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3eac-135">String</span></span>|<span data-ttu-id="e3eac-136">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="e3eac-136">User name.</span></span>|
|<span data-ttu-id="e3eac-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3eac-137">installedDeviceCount</span></span>|<span data-ttu-id="e3eac-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e3eac-138">Int32</span></span>|<span data-ttu-id="e3eac-139">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="e3eac-139">Installed Device Count.</span></span>|
|<span data-ttu-id="e3eac-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3eac-140">failedDeviceCount</span></span>|<span data-ttu-id="e3eac-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e3eac-141">Int32</span></span>|<span data-ttu-id="e3eac-142">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e3eac-142">Failed Device Count.</span></span>|
|<span data-ttu-id="e3eac-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3eac-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="e3eac-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e3eac-144">Int32</span></span>|<span data-ttu-id="e3eac-145">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="e3eac-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="e3eac-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3eac-146">Response</span></span>
<span data-ttu-id="e3eac-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3eac-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3eac-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3eac-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3eac-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3eac-149">Request</span></span>
<span data-ttu-id="e3eac-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3eac-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3eac-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3eac-151">Response</span></span>
<span data-ttu-id="e3eac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3eac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




