---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bbd9174ef791c6f0e5517131d9c757a2e5755e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552816"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="f77ea-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="f77ea-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="f77ea-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f77ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77ea-105">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f77ea-105">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77ea-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f77ea-106">Prerequisites</span></span>
<span data-ttu-id="f77ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f77ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f77ea-109">Permission type</span></span>|<span data-ttu-id="f77ea-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f77ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f77ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f77ea-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77ea-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f77ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f77ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f77ea-114">Not supported.</span></span>|
|<span data-ttu-id="f77ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f77ea-115">Application</span></span>|<span data-ttu-id="f77ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f77ea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f77ea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f77ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f77ea-118">Request headers</span></span>
|<span data-ttu-id="f77ea-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f77ea-119">Header</span></span>|<span data-ttu-id="f77ea-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f77ea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77ea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f77ea-121">Authorization</span></span>|<span data-ttu-id="f77ea-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f77ea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77ea-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f77ea-123">Accept</span></span>|<span data-ttu-id="f77ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f77ea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77ea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f77ea-125">Request body</span></span>
<span data-ttu-id="f77ea-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f77ea-126">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="f77ea-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f77ea-127">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="f77ea-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f77ea-128">Property</span></span>|<span data-ttu-id="f77ea-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f77ea-129">Type</span></span>|<span data-ttu-id="f77ea-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f77ea-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77ea-131">id</span><span class="sxs-lookup"><span data-stu-id="f77ea-131">id</span></span>|<span data-ttu-id="f77ea-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f77ea-132">String</span></span>|<span data-ttu-id="f77ea-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f77ea-133">Key of the entity.</span></span> <span data-ttu-id="f77ea-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f77ea-135">displayName</span></span>|<span data-ttu-id="f77ea-136">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-136">String</span></span>|<span data-ttu-id="f77ea-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f77ea-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f77ea-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-139">description</span><span class="sxs-lookup"><span data-stu-id="f77ea-139">description</span></span>|<span data-ttu-id="f77ea-140">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-140">String</span></span>|<span data-ttu-id="f77ea-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-141">The description of the app.</span></span> <span data-ttu-id="f77ea-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-143">publicador</span><span class="sxs-lookup"><span data-stu-id="f77ea-143">publisher</span></span>|<span data-ttu-id="f77ea-144">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-144">String</span></span>|<span data-ttu-id="f77ea-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-145">The publisher of the app.</span></span> <span data-ttu-id="f77ea-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f77ea-147">largeIcon</span></span>|[<span data-ttu-id="f77ea-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f77ea-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f77ea-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f77ea-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f77ea-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f77ea-151">createdDateTime</span></span>|<span data-ttu-id="f77ea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77ea-152">DateTimeOffset</span></span>|<span data-ttu-id="f77ea-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-153">The date and time the app was created.</span></span> <span data-ttu-id="f77ea-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f77ea-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f77ea-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77ea-156">DateTimeOffset</span></span>|<span data-ttu-id="f77ea-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f77ea-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f77ea-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f77ea-159">isFeatured</span></span>|<span data-ttu-id="f77ea-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f77ea-160">Boolean</span></span>|<span data-ttu-id="f77ea-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f77ea-162">privacyInformationUrl</span></span>|<span data-ttu-id="f77ea-163">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-163">String</span></span>|<span data-ttu-id="f77ea-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f77ea-164">The privacy statement Url.</span></span> <span data-ttu-id="f77ea-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f77ea-166">informationUrl</span></span>|<span data-ttu-id="f77ea-167">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-167">String</span></span>|<span data-ttu-id="f77ea-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f77ea-168">The more information Url.</span></span> <span data-ttu-id="f77ea-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-170">owner</span><span class="sxs-lookup"><span data-stu-id="f77ea-170">owner</span></span>|<span data-ttu-id="f77ea-171">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-171">String</span></span>|<span data-ttu-id="f77ea-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-172">The owner of the app.</span></span> <span data-ttu-id="f77ea-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-174">developer</span><span class="sxs-lookup"><span data-stu-id="f77ea-174">developer</span></span>|<span data-ttu-id="f77ea-175">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-175">String</span></span>|<span data-ttu-id="f77ea-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-176">The developer of the app.</span></span> <span data-ttu-id="f77ea-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-178">notes</span><span class="sxs-lookup"><span data-stu-id="f77ea-178">notes</span></span>|<span data-ttu-id="f77ea-179">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-179">String</span></span>|<span data-ttu-id="f77ea-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-180">Notes for the app.</span></span> <span data-ttu-id="f77ea-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f77ea-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f77ea-182">publishingState</span></span>|[<span data-ttu-id="f77ea-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f77ea-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f77ea-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-184">The publishing state for the app.</span></span> <span data-ttu-id="f77ea-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f77ea-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f77ea-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f77ea-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f77ea-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f77ea-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f77ea-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f77ea-188">appAvailability</span></span>|[<span data-ttu-id="f77ea-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f77ea-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f77ea-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-190">The Application's availability.</span></span> <span data-ttu-id="f77ea-191">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f77ea-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f77ea-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f77ea-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f77ea-193">version</span><span class="sxs-lookup"><span data-stu-id="f77ea-193">version</span></span>|<span data-ttu-id="f77ea-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f77ea-194">String</span></span>|<span data-ttu-id="f77ea-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f77ea-195">The Application's version.</span></span> <span data-ttu-id="f77ea-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f77ea-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f77ea-197">committedContentVersion</span></span>|<span data-ttu-id="f77ea-198">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-198">String</span></span>|<span data-ttu-id="f77ea-199">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f77ea-199">The internal committed content version.</span></span> <span data-ttu-id="f77ea-200">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f77ea-201">fileName</span><span class="sxs-lookup"><span data-stu-id="f77ea-201">fileName</span></span>|<span data-ttu-id="f77ea-202">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-202">String</span></span>|<span data-ttu-id="f77ea-203">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f77ea-203">The name of the main Lob application file.</span></span> <span data-ttu-id="f77ea-204">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f77ea-205">size</span><span class="sxs-lookup"><span data-stu-id="f77ea-205">size</span></span>|<span data-ttu-id="f77ea-206">Int64</span><span class="sxs-lookup"><span data-stu-id="f77ea-206">Int64</span></span>|<span data-ttu-id="f77ea-207">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f77ea-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="f77ea-208">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f77ea-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f77ea-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="f77ea-209">bundleId</span></span>|<span data-ttu-id="f77ea-210">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-210">String</span></span>|<span data-ttu-id="f77ea-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f77ea-211">The Identity Name.</span></span>|
|<span data-ttu-id="f77ea-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f77ea-212">applicableDeviceType</span></span>|[<span data-ttu-id="f77ea-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f77ea-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f77ea-214">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="f77ea-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f77ea-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f77ea-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f77ea-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f77ea-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f77ea-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f77ea-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f77ea-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f77ea-218">expirationDateTime</span></span>|<span data-ttu-id="f77ea-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77ea-219">DateTimeOffset</span></span>|<span data-ttu-id="f77ea-220">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="f77ea-220">The expiration time.</span></span>|
|<span data-ttu-id="f77ea-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="f77ea-221">versionNumber</span></span>|<span data-ttu-id="f77ea-222">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-222">String</span></span>|<span data-ttu-id="f77ea-223">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f77ea-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f77ea-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f77ea-224">buildNumber</span></span>|<span data-ttu-id="f77ea-225">String</span><span class="sxs-lookup"><span data-stu-id="f77ea-225">String</span></span>|<span data-ttu-id="f77ea-226">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f77ea-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="f77ea-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="f77ea-227">Response</span></span>
<span data-ttu-id="f77ea-228">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f77ea-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77ea-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f77ea-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77ea-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f77ea-230">Request</span></span>
<span data-ttu-id="f77ea-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f77ea-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="f77ea-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="f77ea-232">Response</span></span>
<span data-ttu-id="f77ea-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f77ea-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



