---
title: Tipo de enumeração resultantAppState
description: Uma lista de possíveis estados para o status do aplicativo em um dispositivo individual. Quando os dispositivos contatarem o serviço Intune e localizarem a intenção de imposição de aplicativo direcionada, o status da imposição será registrado e ficará acessível no API do Graph. Como o status do aplicativo é identificado durante a interação do dispositivo com o serviço Intune, os registros de status não aparecem imediatamente após a atribuição do grupo de aplicativos; ele é criado somente depois que a atribuição é avaliada no serviço e os dispositivos começam a receber a política durante os check-ins.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5d05a7ac37c525e5a598e158a386dd1d14c35a23
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211923"
---
# <a name="resultantappstate-enum-type"></a>Tipo de enumeração resultantAppState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma lista de possíveis estados para o status do aplicativo em um dispositivo individual. Quando os dispositivos contatarem o serviço Intune e localizarem a intenção de imposição de aplicativo direcionada, o status da imposição será registrado e ficará acessível no API do Graph. Como o status do aplicativo é identificado durante a interação do dispositivo com o serviço Intune, os registros de status não aparecem imediatamente após a atribuição do grupo de aplicativos; ele é criado somente depois que a atribuição é avaliada no serviço e os dispositivos começam a receber a política durante os check-ins.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Instalado|1|O aplicativo é instalado sem erros.|
|Falhou|2|Falha na instalação do aplicativo.|
|notInstalled|3|O aplicativo não está instalado.|
|uninstallFailed|4|Falha ao desinstalar o aplicativo.|
|pendingInstall|5|A instalação do aplicativo está em andamento.|
|desconhecido|99|O status do aplicativo é desconhecido.|
|notApplicable|-1|O aplicativo não é aplicável.|




