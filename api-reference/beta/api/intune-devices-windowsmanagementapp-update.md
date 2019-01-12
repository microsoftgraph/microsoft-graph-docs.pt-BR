---
title: Atualizar windowsManagementApp
description: Atualize as propriedades de um objeto windowsManagementApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fe6412c08ba05bb26985cc5fd6a8ab0b58bc8e59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980241"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="f858c-103">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f858c-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="f858c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f858c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f858c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f858c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f858c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f858c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f858c-107">Atualize as propriedades de um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f858c-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f858c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f858c-108">Prerequisites</span></span>
<span data-ttu-id="f858c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f858c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f858c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f858c-111">Permission type</span></span>|<span data-ttu-id="f858c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f858c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f858c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f858c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f858c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f858c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f858c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f858c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f858c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f858c-116">Not supported.</span></span>|
|<span data-ttu-id="f858c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f858c-117">Application</span></span>|<span data-ttu-id="f858c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f858c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f858c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f858c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="f858c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f858c-120">Request headers</span></span>
|<span data-ttu-id="f858c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f858c-121">Header</span></span>|<span data-ttu-id="f858c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f858c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f858c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f858c-123">Authorization</span></span>|<span data-ttu-id="f858c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f858c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f858c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f858c-125">Accept</span></span>|<span data-ttu-id="f858c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f858c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f858c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f858c-127">Request body</span></span>
<span data-ttu-id="f858c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f858c-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="f858c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="f858c-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="f858c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f858c-130">Property</span></span>|<span data-ttu-id="f858c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f858c-131">Type</span></span>|<span data-ttu-id="f858c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f858c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f858c-133">id</span><span class="sxs-lookup"><span data-stu-id="f858c-133">id</span></span>|<span data-ttu-id="f858c-134">String</span><span class="sxs-lookup"><span data-stu-id="f858c-134">String</span></span>|<span data-ttu-id="f858c-135">Identificador exclusivo para o aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="f858c-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="f858c-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="f858c-136">availableVersion</span></span>|<span data-ttu-id="f858c-137">String</span><span class="sxs-lookup"><span data-stu-id="f858c-137">String</span></span>|<span data-ttu-id="f858c-138">Versão disponível do Windows management app.</span><span class="sxs-lookup"><span data-stu-id="f858c-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="f858c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f858c-139">Response</span></span>
<span data-ttu-id="f858c-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f858c-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f858c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f858c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="f858c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f858c-142">Request</span></span>
<span data-ttu-id="f858c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f858c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 53

{
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="f858c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f858c-144">Response</span></span>
<span data-ttu-id="f858c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f858c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





