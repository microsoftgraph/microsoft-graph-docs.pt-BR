---
title: Gerenciamento de despesas de telecomunicações no Microsoft Intune-API do Microsoft Graph
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) relacionadas ao gerenciamento de despesas de telecomunicações para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 9856f01337d7ed6af6fc6df6c2e3e118b762ca0a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938615"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Gerenciamento de despesas com telecomunicações no Microsoft Intune

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

É possível limitar o uso e o roaming de dados em dispositivos de propriedade corporativa ao usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo, que é integrado ao Intune. O serviço permite configurar e impor limites de uso e enviar aos usuários um alerta quando eles excederem um limite configurado. Também é possível configurar o serviço para realizar outras ações, como a desabilitação do roaming, quando os usuários excederem o limite. Relatórios com informações sobre o uso e o monitoramento dos dados estão disponíveis no console do Saaswedo. Antes de usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo com o Intune, é preciso definir as configurações em um console do Saaswedo e no Intune. A conexão deve ser ativada para o serviço Saaswedo e para o Intune. Se a conexão do lado do Saaswedo estiver habilitada, mas a do lado do Intune não estiver, o Intune receberá a comunicação, mas ela será ignorada.

Os seguintes recursos do Graph estão disponíveis para gerenciar despesas com telecomunicações no Intune:

- [Parceiro de gerenciamento de despesas com telecomunicações](intune-tem-telecomexpensemanagementpartner.md)
