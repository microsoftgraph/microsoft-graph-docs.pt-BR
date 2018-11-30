---
title: Atualizar onPremisesConditionalAccessSettings
description: Atualizar as propriedades de um objeto onPremisesConditionalAccessSettings.
ms.openlocfilehash: 31679b6c698903083675e926fa77e0c56be49a38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041200"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="58a4b-103">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="58a4b-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="58a4b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="58a4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58a4b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58a4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58a4b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="58a4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58a4b-107">Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="58a4b-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58a4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58a4b-108">Prerequisites</span></span>
<span data-ttu-id="58a4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58a4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58a4b-111">Permission type</span></span>|<span data-ttu-id="58a4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58a4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58a4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58a4b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a4b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58a4b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58a4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a4b-116">Not supported.</span></span>|
|<span data-ttu-id="58a4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58a4b-117">Application</span></span>|<span data-ttu-id="58a4b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a4b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58a4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="58a4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58a4b-120">Request headers</span></span>
|<span data-ttu-id="58a4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58a4b-121">Header</span></span>|<span data-ttu-id="58a4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58a4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58a4b-123">Authorization</span></span>|<span data-ttu-id="58a4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58a4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a4b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58a4b-125">Accept</span></span>|<span data-ttu-id="58a4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58a4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58a4b-127">Request body</span></span>
<span data-ttu-id="58a4b-128">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="58a4b-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="58a4b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="58a4b-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="58a4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58a4b-130">Property</span></span>|<span data-ttu-id="58a4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58a4b-131">Type</span></span>|<span data-ttu-id="58a4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58a4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a4b-133">id</span><span class="sxs-lookup"><span data-stu-id="58a4b-133">id</span></span>|<span data-ttu-id="58a4b-134">String</span><span class="sxs-lookup"><span data-stu-id="58a4b-134">String</span></span>|<span data-ttu-id="58a4b-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="58a4b-135">Not yet documented</span></span>|
|<span data-ttu-id="58a4b-136">enabled</span><span class="sxs-lookup"><span data-stu-id="58a4b-136">enabled</span></span>|<span data-ttu-id="58a4b-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="58a4b-137">Boolean</span></span>|<span data-ttu-id="58a4b-138">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="58a4b-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="58a4b-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="58a4b-139">includedGroups</span></span>|<span data-ttu-id="58a4b-140">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="58a4b-140">Guid collection</span></span>|<span data-ttu-id="58a4b-141">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="58a4b-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="58a4b-142">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="58a4b-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="58a4b-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="58a4b-143">excludedGroups</span></span>|<span data-ttu-id="58a4b-144">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="58a4b-144">Guid collection</span></span>|<span data-ttu-id="58a4b-145">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="58a4b-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="58a4b-146">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="58a4b-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="58a4b-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="58a4b-147">overrideDefaultRule</span></span>|<span data-ttu-id="58a4b-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="58a4b-148">Boolean</span></span>|<span data-ttu-id="58a4b-149">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="58a4b-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="58a4b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a4b-150">Response</span></span>
<span data-ttu-id="58a4b-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a4b-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a4b-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58a4b-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="58a4b-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58a4b-153">Request</span></span>
<span data-ttu-id="58a4b-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58a4b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 201

{
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="58a4b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a4b-155">Response</span></span>
<span data-ttu-id="58a4b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58a4b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```





