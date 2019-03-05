---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 562e8c18e0f9cc5a76b78026d23ae413926e5db0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156620"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="b9808-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="b9808-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="b9808-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9808-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9808-106">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9808-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9808-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9808-107">Prerequisites</span></span>
<span data-ttu-id="b9808-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9808-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9808-110">Permission type</span></span>|<span data-ttu-id="b9808-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9808-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9808-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9808-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9808-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9808-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9808-115">Not supported.</span></span>|
|<span data-ttu-id="b9808-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9808-116">Application</span></span>|<span data-ttu-id="b9808-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9808-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9808-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9808-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b9808-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9808-119">Request headers</span></span>
|<span data-ttu-id="b9808-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9808-120">Header</span></span>|<span data-ttu-id="b9808-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b9808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9808-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9808-122">Authorization</span></span>|<span data-ttu-id="b9808-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9808-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9808-124">Accept</span></span>|<span data-ttu-id="b9808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9808-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9808-126">Request body</span></span>
<span data-ttu-id="b9808-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="b9808-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="b9808-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="b9808-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="b9808-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9808-129">Property</span></span>|<span data-ttu-id="b9808-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9808-130">Type</span></span>|<span data-ttu-id="b9808-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9808-132">id</span><span class="sxs-lookup"><span data-stu-id="b9808-132">id</span></span>|<span data-ttu-id="b9808-133">String</span><span class="sxs-lookup"><span data-stu-id="b9808-133">String</span></span>|<span data-ttu-id="b9808-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b9808-134">Key of the entity.</span></span> <span data-ttu-id="b9808-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b9808-136">displayName</span></span>|<span data-ttu-id="b9808-137">String</span><span class="sxs-lookup"><span data-stu-id="b9808-137">String</span></span>|<span data-ttu-id="b9808-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b9808-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b9808-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-140">description</span><span class="sxs-lookup"><span data-stu-id="b9808-140">description</span></span>|<span data-ttu-id="b9808-141">String</span><span class="sxs-lookup"><span data-stu-id="b9808-141">String</span></span>|<span data-ttu-id="b9808-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-142">The description of the app.</span></span> <span data-ttu-id="b9808-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b9808-144">publisher</span></span>|<span data-ttu-id="b9808-145">String</span><span class="sxs-lookup"><span data-stu-id="b9808-145">String</span></span>|<span data-ttu-id="b9808-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-146">The publisher of the app.</span></span> <span data-ttu-id="b9808-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b9808-148">largeIcon</span></span>|[<span data-ttu-id="b9808-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b9808-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b9808-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b9808-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b9808-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9808-152">createdDateTime</span></span>|<span data-ttu-id="b9808-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9808-153">DateTimeOffset</span></span>|<span data-ttu-id="b9808-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-154">The date and time the app was created.</span></span> <span data-ttu-id="b9808-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9808-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b9808-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9808-157">DateTimeOffset</span></span>|<span data-ttu-id="b9808-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b9808-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b9808-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b9808-160">isFeatured</span></span>|<span data-ttu-id="b9808-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9808-161">Boolean</span></span>|<span data-ttu-id="b9808-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b9808-163">privacyInformationUrl</span></span>|<span data-ttu-id="b9808-164">String</span><span class="sxs-lookup"><span data-stu-id="b9808-164">String</span></span>|<span data-ttu-id="b9808-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b9808-165">The privacy statement Url.</span></span> <span data-ttu-id="b9808-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b9808-167">informationUrl</span></span>|<span data-ttu-id="b9808-168">String</span><span class="sxs-lookup"><span data-stu-id="b9808-168">String</span></span>|<span data-ttu-id="b9808-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b9808-169">The more information Url.</span></span> <span data-ttu-id="b9808-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-171">owner</span><span class="sxs-lookup"><span data-stu-id="b9808-171">owner</span></span>|<span data-ttu-id="b9808-172">String</span><span class="sxs-lookup"><span data-stu-id="b9808-172">String</span></span>|<span data-ttu-id="b9808-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b9808-173">The owner of the app.</span></span> <span data-ttu-id="b9808-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-175">developer</span><span class="sxs-lookup"><span data-stu-id="b9808-175">developer</span></span>|<span data-ttu-id="b9808-176">String</span><span class="sxs-lookup"><span data-stu-id="b9808-176">String</span></span>|<span data-ttu-id="b9808-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-177">The developer of the app.</span></span> <span data-ttu-id="b9808-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-179">Observações</span><span class="sxs-lookup"><span data-stu-id="b9808-179">notes</span></span>|<span data-ttu-id="b9808-180">String</span><span class="sxs-lookup"><span data-stu-id="b9808-180">String</span></span>|<span data-ttu-id="b9808-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-181">Notes for the app.</span></span> <span data-ttu-id="b9808-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b9808-183">uploadState</span></span>|<span data-ttu-id="b9808-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b9808-184">Int32</span></span>|<span data-ttu-id="b9808-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b9808-185">The upload state.</span></span> <span data-ttu-id="b9808-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b9808-187">publishingState</span></span>|[<span data-ttu-id="b9808-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b9808-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b9808-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-189">The publishing state for the app.</span></span> <span data-ttu-id="b9808-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b9808-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b9808-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9808-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b9808-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b9808-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b9808-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b9808-193">isAssigned</span></span>|<span data-ttu-id="b9808-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9808-194">Boolean</span></span>|<span data-ttu-id="b9808-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b9808-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b9808-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9808-197">roleScopeTagIds</span></span>|<span data-ttu-id="b9808-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9808-198">String collection</span></span>|<span data-ttu-id="b9808-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b9808-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b9808-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9808-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b9808-201">appAvailability</span></span>|[<span data-ttu-id="b9808-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b9808-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b9808-203">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-203">The Application's availability.</span></span> <span data-ttu-id="b9808-204">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9808-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="b9808-205">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b9808-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b9808-206">version</span><span class="sxs-lookup"><span data-stu-id="b9808-206">version</span></span>|<span data-ttu-id="b9808-207">String</span><span class="sxs-lookup"><span data-stu-id="b9808-207">String</span></span>|<span data-ttu-id="b9808-208">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b9808-208">The Application's version.</span></span> <span data-ttu-id="b9808-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9808-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="b9808-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="b9808-210">bundleId</span></span>|<span data-ttu-id="b9808-211">String</span><span class="sxs-lookup"><span data-stu-id="b9808-211">String</span></span>|<span data-ttu-id="b9808-212">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b9808-212">The app's Bundle ID.</span></span>|
|<span data-ttu-id="b9808-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b9808-213">appStoreUrl</span></span>|<span data-ttu-id="b9808-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9808-214">String</span></span>|<span data-ttu-id="b9808-215">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="b9808-215">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="b9808-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b9808-216">applicableDeviceType</span></span>|[<span data-ttu-id="b9808-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b9808-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b9808-218">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b9808-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="b9808-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b9808-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b9808-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b9808-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="b9808-221">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="b9808-221">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b9808-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9808-222">Response</span></span>
<span data-ttu-id="b9808-223">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9808-223">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9808-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9808-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9808-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9808-225">Request</span></span>
<span data-ttu-id="b9808-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9808-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b9808-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9808-227">Response</span></span>
<span data-ttu-id="b9808-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9808-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1363

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```




