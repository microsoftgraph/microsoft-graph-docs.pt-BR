---
title: Atualizar windowsManagementApp
description: Atualize as propriedades de um objeto windowsManagementApp.
ms.openlocfilehash: 88a0511a06c94a4c5298fc53fa19b512f723177d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034786"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="905e2-103">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="905e2-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="905e2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="905e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="905e2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="905e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="905e2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="905e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="905e2-107">Atualize as propriedades de um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="905e2-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="905e2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="905e2-108">Prerequisites</span></span>
<span data-ttu-id="905e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="905e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="905e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="905e2-111">Permission type</span></span>|<span data-ttu-id="905e2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="905e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="905e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="905e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="905e2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="905e2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="905e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="905e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="905e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="905e2-116">Not supported.</span></span>|
|<span data-ttu-id="905e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="905e2-117">Application</span></span>|<span data-ttu-id="905e2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="905e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="905e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="905e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="905e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="905e2-120">Request headers</span></span>
|<span data-ttu-id="905e2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="905e2-121">Header</span></span>|<span data-ttu-id="905e2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="905e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="905e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="905e2-123">Authorization</span></span>|<span data-ttu-id="905e2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="905e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="905e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="905e2-125">Accept</span></span>|<span data-ttu-id="905e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="905e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="905e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="905e2-127">Request body</span></span>
<span data-ttu-id="905e2-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="905e2-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="905e2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="905e2-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="905e2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="905e2-130">Property</span></span>|<span data-ttu-id="905e2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="905e2-131">Type</span></span>|<span data-ttu-id="905e2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="905e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="905e2-133">id</span><span class="sxs-lookup"><span data-stu-id="905e2-133">id</span></span>|<span data-ttu-id="905e2-134">String</span><span class="sxs-lookup"><span data-stu-id="905e2-134">String</span></span>|<span data-ttu-id="905e2-135">Identificador exclusivo para o aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="905e2-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="905e2-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="905e2-136">availableVersion</span></span>|<span data-ttu-id="905e2-137">String</span><span class="sxs-lookup"><span data-stu-id="905e2-137">String</span></span>|<span data-ttu-id="905e2-138">Versão disponível do Windows management app.</span><span class="sxs-lookup"><span data-stu-id="905e2-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="905e2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="905e2-139">Response</span></span>
<span data-ttu-id="905e2-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="905e2-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="905e2-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="905e2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="905e2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="905e2-142">Request</span></span>
<span data-ttu-id="905e2-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="905e2-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 53

{
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="905e2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="905e2-144">Response</span></span>
<span data-ttu-id="905e2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="905e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```





