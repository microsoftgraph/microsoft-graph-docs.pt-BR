---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0ac3ad93fa6847ce62b6710286fc6eec977c66d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819506"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="2a191-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="2a191-103">Update iosVppApp</span></span>

> <span data-ttu-id="2a191-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2a191-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a191-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2a191-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a191-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a191-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a191-107">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a191-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a191-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a191-108">Prerequisites</span></span>
<span data-ttu-id="2a191-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a191-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a191-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a191-111">Permission type</span></span>|<span data-ttu-id="2a191-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a191-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a191-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a191-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a191-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a191-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a191-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a191-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a191-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a191-116">Not supported.</span></span>|
|<span data-ttu-id="2a191-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a191-117">Application</span></span>|<span data-ttu-id="2a191-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a191-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a191-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a191-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2a191-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a191-120">Request headers</span></span>
|<span data-ttu-id="2a191-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a191-121">Header</span></span>|<span data-ttu-id="2a191-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2a191-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a191-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a191-123">Authorization</span></span>|<span data-ttu-id="2a191-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a191-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a191-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a191-125">Accept</span></span>|<span data-ttu-id="2a191-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a191-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a191-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a191-127">Request body</span></span>
<span data-ttu-id="2a191-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a191-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="2a191-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a191-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="2a191-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a191-130">Property</span></span>|<span data-ttu-id="2a191-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a191-131">Type</span></span>|<span data-ttu-id="2a191-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a191-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a191-133">id</span><span class="sxs-lookup"><span data-stu-id="2a191-133">id</span></span>|<span data-ttu-id="2a191-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-134">String</span></span>|<span data-ttu-id="2a191-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a191-135">Key of the entity.</span></span> <span data-ttu-id="2a191-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2a191-137">displayName</span></span>|<span data-ttu-id="2a191-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-138">String</span></span>|<span data-ttu-id="2a191-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2a191-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a191-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-141">description</span><span class="sxs-lookup"><span data-stu-id="2a191-141">description</span></span>|<span data-ttu-id="2a191-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-142">String</span></span>|<span data-ttu-id="2a191-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-143">The description of the app.</span></span> <span data-ttu-id="2a191-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2a191-145">publisher</span></span>|<span data-ttu-id="2a191-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-146">String</span></span>|<span data-ttu-id="2a191-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-147">The publisher of the app.</span></span> <span data-ttu-id="2a191-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a191-149">largeIcon</span></span>|[<span data-ttu-id="2a191-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a191-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2a191-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2a191-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a191-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a191-153">createdDateTime</span></span>|<span data-ttu-id="2a191-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a191-154">DateTimeOffset</span></span>|<span data-ttu-id="2a191-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-155">The date and time the app was created.</span></span> <span data-ttu-id="2a191-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a191-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2a191-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a191-158">DateTimeOffset</span></span>|<span data-ttu-id="2a191-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2a191-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2a191-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a191-161">isFeatured</span></span>|<span data-ttu-id="2a191-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="2a191-162">Boolean</span></span>|<span data-ttu-id="2a191-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a191-164">privacyInformationUrl</span></span>|<span data-ttu-id="2a191-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-165">String</span></span>|<span data-ttu-id="2a191-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2a191-166">The privacy statement Url.</span></span> <span data-ttu-id="2a191-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a191-168">informationUrl</span></span>|<span data-ttu-id="2a191-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-169">String</span></span>|<span data-ttu-id="2a191-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2a191-170">The more information Url.</span></span> <span data-ttu-id="2a191-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-172">owner</span><span class="sxs-lookup"><span data-stu-id="2a191-172">owner</span></span>|<span data-ttu-id="2a191-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-173">String</span></span>|<span data-ttu-id="2a191-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2a191-174">The owner of the app.</span></span> <span data-ttu-id="2a191-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-176">developer</span><span class="sxs-lookup"><span data-stu-id="2a191-176">developer</span></span>|<span data-ttu-id="2a191-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-177">String</span></span>|<span data-ttu-id="2a191-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-178">The developer of the app.</span></span> <span data-ttu-id="2a191-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-180">Observações</span><span class="sxs-lookup"><span data-stu-id="2a191-180">notes</span></span>|<span data-ttu-id="2a191-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-181">String</span></span>|<span data-ttu-id="2a191-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-182">Notes for the app.</span></span> <span data-ttu-id="2a191-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2a191-184">uploadState</span></span>|<span data-ttu-id="2a191-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2a191-185">Int32</span></span>|<span data-ttu-id="2a191-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="2a191-186">The upload state.</span></span> <span data-ttu-id="2a191-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a191-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a191-188">publishingState</span></span>|[<span data-ttu-id="2a191-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2a191-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2a191-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-190">The publishing state for the app.</span></span> <span data-ttu-id="2a191-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2a191-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a191-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a191-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2a191-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2a191-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2a191-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2a191-194">usedLicenseCount</span></span>|<span data-ttu-id="2a191-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2a191-195">Int32</span></span>|<span data-ttu-id="2a191-196">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="2a191-196">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2a191-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2a191-197">totalLicenseCount</span></span>|<span data-ttu-id="2a191-198">Int32</span><span class="sxs-lookup"><span data-stu-id="2a191-198">Int32</span></span>|<span data-ttu-id="2a191-199">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="2a191-199">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2a191-200">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="2a191-200">releaseDateTime</span></span>|<span data-ttu-id="2a191-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a191-201">DateTimeOffset</span></span>|<span data-ttu-id="2a191-202">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="2a191-202">The VPP application release date and time.</span></span>|
|<span data-ttu-id="2a191-203">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2a191-203">appStoreUrl</span></span>|<span data-ttu-id="2a191-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-204">String</span></span>|<span data-ttu-id="2a191-205">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="2a191-205">The store URL.</span></span>|
|<span data-ttu-id="2a191-206">licensingType</span><span class="sxs-lookup"><span data-stu-id="2a191-206">licensingType</span></span>|[<span data-ttu-id="2a191-207">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2a191-207">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2a191-208">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="2a191-208">The supported License Type.</span></span>|
|<span data-ttu-id="2a191-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a191-209">applicableDeviceType</span></span>|[<span data-ttu-id="2a191-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a191-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2a191-211">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="2a191-211">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="2a191-212">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2a191-212">vppTokenOrganizationName</span></span>|<span data-ttu-id="2a191-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-213">String</span></span>|<span data-ttu-id="2a191-214">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="2a191-214">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2a191-215">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2a191-215">vppTokenAccountType</span></span>|[<span data-ttu-id="2a191-216">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2a191-216">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2a191-217">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="2a191-217">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2a191-218">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2a191-218">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2a191-219">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2a191-219">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2a191-220">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="2a191-220">vppTokenAppleId</span></span>|<span data-ttu-id="2a191-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-221">String</span></span>|<span data-ttu-id="2a191-222">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="2a191-222">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2a191-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="2a191-223">bundleId</span></span>|<span data-ttu-id="2a191-224">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-224">String</span></span>|<span data-ttu-id="2a191-225">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2a191-225">The Identity Name.</span></span>|
|<span data-ttu-id="2a191-226">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2a191-226">vppTokenId</span></span>|<span data-ttu-id="2a191-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a191-227">String</span></span>|<span data-ttu-id="2a191-228">Identificador do token VPP associado a esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-228">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="2a191-229">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="2a191-229">revokeLicenseActionResults</span></span>|<span data-ttu-id="2a191-230">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2a191-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="2a191-231">Resultados de revogar ações de licença em deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a191-231">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="2a191-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a191-232">Response</span></span>
<span data-ttu-id="2a191-233">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a191-233">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a191-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a191-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a191-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a191-235">Request</span></span>
<span data-ttu-id="2a191-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a191-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1903

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2a191-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a191-237">Response</span></span>
<span data-ttu-id="2a191-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a191-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2059

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```





