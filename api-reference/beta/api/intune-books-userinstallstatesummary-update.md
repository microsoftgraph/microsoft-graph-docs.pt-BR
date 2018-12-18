---
title: Atualizar userInstallStateSummary
description: Atualizar as propriedades de um objeto userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: 10129a9a18030498add1b8e3c0b664f2aa921de6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316461"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="515cd-103">Atualizar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="515cd-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="515cd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="515cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="515cd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="515cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="515cd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="515cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="515cd-107">Atualizar as propriedades de um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="515cd-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="515cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="515cd-108">Prerequisites</span></span>
<span data-ttu-id="515cd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="515cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="515cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="515cd-111">Permission type</span></span>|<span data-ttu-id="515cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="515cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="515cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="515cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="515cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="515cd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="515cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="515cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="515cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="515cd-116">Not supported.</span></span>|
|<span data-ttu-id="515cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="515cd-117">Application</span></span>|<span data-ttu-id="515cd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="515cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="515cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="515cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="515cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="515cd-120">Request headers</span></span>
|<span data-ttu-id="515cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="515cd-121">Header</span></span>|<span data-ttu-id="515cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="515cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="515cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="515cd-123">Authorization</span></span>|<span data-ttu-id="515cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="515cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="515cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="515cd-125">Accept</span></span>|<span data-ttu-id="515cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="515cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="515cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="515cd-127">Request body</span></span>
<span data-ttu-id="515cd-128">No corpo da solicitação, forneça uma representação JSON do objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="515cd-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="515cd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="515cd-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="515cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="515cd-130">Property</span></span>|<span data-ttu-id="515cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="515cd-131">Type</span></span>|<span data-ttu-id="515cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="515cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="515cd-133">id</span><span class="sxs-lookup"><span data-stu-id="515cd-133">id</span></span>|<span data-ttu-id="515cd-134">String</span><span class="sxs-lookup"><span data-stu-id="515cd-134">String</span></span>|<span data-ttu-id="515cd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="515cd-135">Key of the entity.</span></span>|
|<span data-ttu-id="515cd-136">userName</span><span class="sxs-lookup"><span data-stu-id="515cd-136">userName</span></span>|<span data-ttu-id="515cd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="515cd-137">String</span></span>|<span data-ttu-id="515cd-138">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="515cd-138">User name.</span></span>|
|<span data-ttu-id="515cd-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="515cd-139">installedDeviceCount</span></span>|<span data-ttu-id="515cd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="515cd-140">Int32</span></span>|<span data-ttu-id="515cd-141">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="515cd-141">Installed Device Count.</span></span>|
|<span data-ttu-id="515cd-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="515cd-142">failedDeviceCount</span></span>|<span data-ttu-id="515cd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="515cd-143">Int32</span></span>|<span data-ttu-id="515cd-144">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="515cd-144">Failed Device Count.</span></span>|
|<span data-ttu-id="515cd-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="515cd-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="515cd-146">Int32</span><span class="sxs-lookup"><span data-stu-id="515cd-146">Int32</span></span>|<span data-ttu-id="515cd-147">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="515cd-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="515cd-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="515cd-148">Response</span></span>
<span data-ttu-id="515cd-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="515cd-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="515cd-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="515cd-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="515cd-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="515cd-151">Request</span></span>
<span data-ttu-id="515cd-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="515cd-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 127

{
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="515cd-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="515cd-153">Response</span></span>
<span data-ttu-id="515cd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="515cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





